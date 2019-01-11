---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 6a4f15266ebfda3e2af43a5d39e28803fe9d87b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837370"
---
# <a name="outlookuser-resource-type"></a>Tipo de recurso outlookUser


Representa os serviços do Outlook disponíveis para um usuário.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar categoria](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.|
|[Listar categorias](../api/outlookuser-list-mastercategories.md) | Coleção [outlookCategory](outlookcategory.md) |Obtém todas as categorias que foram definidas para o usuário.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | Coleção [localeInfo](localeinfo.md) | Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário. |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | Coleção [timeZoneInformation](timezoneinformation.md) | Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário. |


## <a name="properties"></a>Propriedades
Nenhum

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|masterCategories|Coleção [outlookCategory](../resources/outlookcategory.md)| Uma lista de categorias definidas para o usuário. | 

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookUser",
  "@odata.annotations": [
    {
      "property": "masterCategories",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
