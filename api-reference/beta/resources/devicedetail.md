---
title: tipo de recurso de deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para assinar. Inclui informações como o navegador do dispositivo e informações do sistema operacional, se o dispositivo for Azure AD gerenciado.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18d55e397cf6c892cd37aea930d446c630017a92
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971358"
---
# <a name="devicedetail-resource-type"></a>tipo de recurso de deviceDetail
Indica os detalhes do dispositivo associados a um dispositivo usado para assinar. Inclui informações como o navegador do dispositivo e informações do sistema operacional, se o dispositivo for Azure AD gerenciado.



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Navegador|Cadeia de caracteres|Indica as informações do navegador dos usados para entrar no serviço.|
|deviceId|Cadeia de caracteres|Refere-se o UniqueID do dispositivo usado para entrar no serviço.|
|displayName|Cadeia de caracteres|Refere-se com o nome do dispositivo usado para entrar no serviço.|
|isCompliant|Booliano|Indica se o dispositivo é compatível com ou não.|
|isManaged|Booliano|Indica se o dispositivo é gerenciado ou não.|
|operatingSystem|Cadeia de caracteres|Indica o nome do sistema operacional e versão usada para entrar no serviço.|
|trustType|Cadeia de caracteres|Indica se o dispositivo conectado é integrado ao domínio local de trabalho associado, AzureAD ingressado, as informações. |

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
