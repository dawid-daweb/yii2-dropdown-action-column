�������������� yii\grid\ActionColumn ��� yii2
=================================

[English readme](https://github.com/microinginer/yii2-dropdown-action-column/blob/master/README.md)

##��������� �� ���������

```php
echo \yii\grid\GridView::widget([
    ...
    'columns'      => [
        ...
        [
            'class' => \microinginer\dropDownActionColumn\DropDownActionColumn::className(),
        ],
    ],
]);
```

![������ yii\grid\ActionColumn ��������� ���������](https://raw.githubusercontent.com/microinginer/yii2-dropdown-action-column/master/screenshots/default-buttons.png "������ yii\grid\ActionColumn ��������� ���������")


##���������������� ������

```php
echo \yii\grid\GridView::widget([
    ...
    'columns'      => [
        ...
        [
            'class' => \microinginer\dropDownActionColumn\DropDownActionColumn::className(),
            'items' => [
                [
                    'label' => 'View',
                    'url'   => ['view'],
                ],
                [
                    'label' => 'Export',
                    'url'   => ['expert'],
                ],
                [
                    'label'   => 'Disable',
                    'url'     => ['disable'],
                    'linkOptions' => [
                        'data-method' => 'post'
                    ],
                ],
            ]
        ],
    ],
]);
```

![������ yii\grid\ActionColumn](https://raw.githubusercontent.com/microinginer/yii2-dropdown-action-column/master/screenshots/custom-buttons.png "������ yii\grid\ActionColumn")


##Install

���������������� ������ ��������� [composer](http://getcomposer.org/download/).

��������� ��������

```
php composer.phar require --prefer-dist microinginer/yii2-dropdown-action-column "dev-master"
```

��� �������

```json
"microinginer/yii2-dropdown-action-column": "dev-master"
```

� ������ `require` � ����� composer.json �����.