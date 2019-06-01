---
title: tipo de recurso deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para entrar. Inclui informações como navegador de dispositivo e informações de so, se o dispositivo for gerenciado pelo Azure AD.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f3a0d7f141723beb5194860b025fe6fa349eb95a
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657697"
---
# <a name="devicedetail-resource-type"></a>tipo de recurso deviceDetail
Indica os detalhes do dispositivo associados a um dispositivo usado para entrar. Inclui informações como navegador de dispositivo e informações de so, se o dispositivo for gerenciado pelo Azure AD.



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Navegador|String|Indica as informações do navegador do usado para entrar.|
|deviceId|String|Refere-se ao UniqueID do dispositivo usado para entrar.|
|displayName|String|Refere-se ao nome do dispositivo usado para entrar.|
|isCompliant|Booliano|Indica se o dispositivo está em conformidade ou não.|
|isManaged|Booliano|Indica se o dispositivo é gerenciado ou não.|
|operatingSystem|Cadeia de caracteres|Indica o nome do sistema operacional e a versão usada para entrar.|
|trustType|String|Indica informações sobre se o dispositivo conectado é membro do local de trabalho, AzureAD Unido, ingresso no domínio. |

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
