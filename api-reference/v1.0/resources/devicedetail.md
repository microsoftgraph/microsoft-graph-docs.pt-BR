---
title: Tipo de recurso deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para entrar. Isso inclui informações como navegador de dispositivo e sistema operacional e se o dispositivo é gerenciado pelo Azure AD.
ms.localizationpriority: medium
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 91710dc5079bc879b8b23a8a3f5b621f4ecc1968
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089820"
---
# <a name="devicedetail-resource-type"></a>Tipo de recurso deviceDetail

Namespace: microsoft.graph

Indica os detalhes do dispositivo associados a um dispositivo usado para entrar. Isso inclui informações como navegador de dispositivo e sistema operacional e se o dispositivo é gerenciado pelo Azure AD.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Navegador|String|Indica as informações do navegador do usado para entrar.|
|deviceId|Cadeia de caracteres|Refere-se ao UniqueID do dispositivo usado para entrar.|
|displayName|Cadeia de caracteres|Refere-se ao nome do dispositivo usado para entrar.|
|isCompliant|Booliano|Indica se o dispositivo é compatível.|
|isManaged|Booliano|Indica se o dispositivo é gerenciado.|
|operatingSystem|String|Indica o nome e a versão do sistema operacional usados para entrar.|
|trustType|String|Fornece informações sobre se o dispositivo conectado é Workplace Joined, AzureAD Joined, Domain Joined. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "browser": "String",
  "deviceId": "String",
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "operatingSystem": "String",
  "trustType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

