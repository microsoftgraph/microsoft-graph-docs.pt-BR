---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: fd2cd782fafbcff4c3006bea22c659c6607bf11a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137001"
---
# <a name="outlookuser-resource-type"></a>Tipo de recurso outlookUser

Namespace: microsoft.graph


Representa os serviços do Outlook disponíveis para um usuário.


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar categoria](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.|
|[Listar categorias](../api/outlookuser-list-mastercategories.md) | Coleção [outlookCategory](outlookcategory.md) |Obtém todas as categorias que foram definidas para o usuário.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | Coleção [localeInfo](localeinfo.md) | Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário. |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | Coleção [timeZoneInformation](timezoneinformation.md) | Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário. |


## <a name="properties"></a>Propriedades
Nenhuma

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

