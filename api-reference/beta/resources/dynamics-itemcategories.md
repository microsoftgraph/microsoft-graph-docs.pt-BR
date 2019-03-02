---
title: tipo de recurso doCategories
description: Uma categoria de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e18319683f6dbceddccc9cf83e48cd3ef89f895d
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365742"
---
# <a name="itemcategories-resource-type"></a>tipo de recurso doCategories
Representa uma categoria de vários itens no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método                                                          | Tipo de retorno  |Descrição             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[Obter as categorias](../api/dynamics-itemcategories-get.md)      |Categoria de|Obtenha uma categoria de item.   |
|[Postar categorias](../api/dynamics-create-itemcategories.md)  |Categoria de|Criar uma categoria de item.|
|[Patch, categorias](../api/dynamics-itemcategories-update.md) |Categoria de|Atualize uma categoria de item.|
|[Excluir myCategories](../api/dynamics-itemcategories-delete.md)|Nenhuma          |Excluir uma categoria de item.|

## <a name="properties"></a>Propriedades
| Propriedade           | Tipo   |Descrição                                     |
|:-------------------|:-------|:-----------------------------------------------|
|id                  |GUID    |A ID exclusiva do mycategory. Não editável.|
|código                |string  |O código de categoria.                          |
|displayName         |string  |O nome de exibição de doCategorias.                |
|lastModifiedDateTime|DateTime|A última data e hora em que a categoria foi modificada. Somente Leitura.|  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON das categorias.

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

