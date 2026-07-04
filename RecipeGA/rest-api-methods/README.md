# API Методы

## Добавить новый продукт с КБЖУ
POST /products


## Создать рецепт пользователем
POST /recipes
с авторизацией пользователя в заголовке header запроса


## Изменить обложку (фото) конкретного рецепта
PATCH /recipes/{recipeId}/cover

### Вариант реализации
Отдельный метод POST /images на загрузку изображений в файловое хранилище, из которого можно получить url для подстановки в "coverUrl"

PATCH /recipes/{recipeId}
с телом { "coverUrl": "..." }


## Удалить продукт из справочника
PATCH /products/{productId}/archive


## Удалить продукт из рецепта (ингредиент)
DELETE /recipes/{recipeId}/ingredients/{ingredientId}
