---
title: tipo de recurso docategories
description: Uma categoria de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 866fda60aa8b0a357e8e587d105a7fa00e116d3d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013836"
---
# <a name="itemcategories-resource-type"></a>tipo de recurso docategories

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma categoria de vários itens no Dynamics 365 Business central.

## <a name="methods"></a>Methods

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
|código                |cadeia de caracteres  |O código de categoria.                          |
|displayName         |string  |O nome de exibição de docategorias.                |
|lastModifiedDateTime|datetime|A última data e hora em que a categoria foi modificada. Somente leitura.|  


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



