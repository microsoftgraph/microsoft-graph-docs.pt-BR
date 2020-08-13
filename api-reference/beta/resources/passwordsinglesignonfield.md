---
title: tipo de recurso passwordSingleSignOnField
description: Campos para capturar as credenciais para SSO de senha
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e20bcd2b9ddeab5ce255285fb6e13af5acb72fce
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658170"
---
# <a name="passwordsinglesignonfield-resource-type"></a>tipo de recurso passwordSingleSignOnField

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém os campos a serem capturados para preencher as credenciais de uso para logon único baseado em senha.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|customizedLabel|String|Substituição de título/rótulo para personalização.|
|defaultlabel|String|Rótulo que seria usado se nenhum customizedLabel for fornecido. Somente leitura.|
|fieldId|String|ID usada para identificar o tipo de campo. Esta é uma ID interna e os valores possíveis são:,, `param_1` `param_2` `param_userName` `param_password` .|
|type|String|   Tipo da credencial. Os valores podem ser `text` , `password` .|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnField",
  "baseType": null
}-->

```json
{
  "customizedLabel": "String",
  "defaultLabel": "String",
  "fieldId": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->