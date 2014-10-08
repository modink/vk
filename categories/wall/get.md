---
layout: default
title: Метод Wall.Get
permalink: wall/get/
comments: true
---
# Метод Wall.Get
Возвращает список записей со стены пользователя или сообщества.

## Синтаксис
```csharp
public ReadOnlyCollection<Post> Get(long ownerId, out int totalCount, int? count = null, int? offset = null, WallFilter filter)
```

## Параметры
+ **ownerId** - Идентификатор поьзователя. Чтобы получить записи со стены группы (публичной страницы, встречи), укажите её идентификатор со знаком "минус": например, owner_id=-1 соответствует группе с идентификатором 1.
+ **totalCount** - Общее количество записей на стене.
+ **count** - Количество сообщений, которое необходимо получить (но не более 100).
+ **offset** - Смещение, необходимое для выборки определенного подмножества сообщений.
+ **filter** - Типы сообщений, которые необходимо получить (по умолчанию возвращаются все сообщения).

## Результат
В случае успеха возвращается запрошенный список записей со стены.

## Исключения

## Пример
```csharp
// TODO:
```