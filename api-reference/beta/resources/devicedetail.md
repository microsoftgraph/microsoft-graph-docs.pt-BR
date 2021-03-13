---
title: Tipo de recurso deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para entrar.
localization_priority: Normal
author: spunukol
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3fb6b338793b77e3079922cd8c372e402488a22c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761125"
---
# <a name="devicedetail-resource-type"></a>Tipo de recurso deviceDetail

Namespace: microsoft.graph Indica detalhes do dispositivo associados a um dispositivo usado para entrar. Inclui informações como navegador de dispositivos e informações do sistema operacional, se o dispositivo for gerenciado pelo Azure AD.



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Navegador|Cadeia de Caracteres|Indica as informações do navegador do usado para entrar.|
|deviceId|Cadeia de caracteres|Refere-se à UniqueID do dispositivo usado para entrar.|
|displayName|Cadeia de caracteres|Refere-se ao nome do dispositivo usado para entrar.|
|isCompliant|Booliano|Indica se o dispositivo está em conformidade ou não.|
|isManaged|Booliano|Indica se o dispositivo é gerenciado ou não.|
|operatingSystem|String|Indica o nome e a versão do sistema operacional usados para entrar.|
|trustType|String|Indica informações sobre se o dispositivo conectado é Workplace Joined, AzureAD Joined, Domain Joined. |

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


