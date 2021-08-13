---
title: Tipo de recurso deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para entrar. Isso inclui informações como navegador de dispositivo e sistema operacional e se o dispositivo é gerenciado pelo Azure AD.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 56522ef5ea6a3404298c776ebdbeebe97c42b2818edfd953af66b050bf793dbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126659"
---
# <a name="devicedetail-resource-type"></a>Tipo de recurso deviceDetail

Namespace: microsoft.graph

Indica os detalhes do dispositivo associados a um dispositivo usado para entrar. Isso inclui informações como navegador de dispositivo e sistema operacional e se o dispositivo é gerenciado pelo Azure AD.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Navegador|Cadeia de caracteres|Indica as informações do navegador do usado para entrar.|
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

