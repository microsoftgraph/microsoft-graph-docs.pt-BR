---
title: tipo de recurso deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para entrar. Isso inclui informações como navegador de dispositivos e sistema operacional e se o dispositivo é gerenciado pelo Azure AD.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a756df15be02544f843e6176677f26ea7e95678
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018698"
---
# <a name="devicedetail-resource-type"></a>tipo de recurso deviceDetail

Namespace: microsoft.graph

Indica os detalhes do dispositivo associados a um dispositivo usado para entrar. Isso inclui informações como navegador de dispositivos e sistema operacional e se o dispositivo é gerenciado pelo Azure AD.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Navegador|String|Indica as informações do navegador do usado para entrar.|
|deviceId|Cadeia de caracteres|Refere-se ao UniqueID do dispositivo usado para entrar.|
|displayName|String|Refere-se ao nome do dispositivo usado para entrar.|
|isCompliant|Booliano|Indica se o dispositivo está em conformidade.|
|isManaged|Booliano|Indica se o dispositivo é gerenciado.|
|operatingSystem|String|Indica o nome do sistema operacional e a versão usada para entrar.|
|trustType|String|Fornece informações sobre se o dispositivo conectado é um local de trabalho associado, AzureAD Unido, ingresso no domínio. |

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

