---
title: Tipo de recurso passwordSingleSignOnField
description: Campos para capturar as credenciais para SSO de senha
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e0db6198d61715603acee54e7351c9fd5f2fed88
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761546"
---
# <a name="passwordsinglesignonfield-resource-type"></a>Tipo de recurso passwordSingleSignOnField

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém os campos a ser capturados para preencher as credenciais de uso para o login único baseado em senha.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|customizedLabel|Cadeia de Caracteres|Substituição de título/rótulo para personalização.|
|defaultLabel|Cadeia de Caracteres|Rótulo que seria usado se nenhum rótulo personalizado for fornecido. Somente leitura.|
|fieldId|Cadeia de Caracteres|ID usada para identificar o tipo de campo. Esta é uma ID interna e os valores possíveis `param_1` são , , , `param_2` `param_userName` `param_password` .|
|tipo|Cadeia de caracteres|   Tipo da credencial. Os valores podem ser `text` , `password` .|

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

