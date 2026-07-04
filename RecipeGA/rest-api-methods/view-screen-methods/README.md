# API Методы экрана просмтотра конкретного рецепта

## Получение информации о рецепте по его id
GET {baseURL}/API/users-app/v1/recipes/{recipeId}/

## Получение комментариев о рецепте по его id
GET {baseURL}/API/users-app/v1/recipes/{recipeId}/comments
>Добавить логику пагинации по 10 комментариев с сортировкой по дате добавления, сначала новые

## Добавление комментария к рецепту по его id
POST {baseURL}/API/users-app/v1/recipes/{recipeId}/comments
