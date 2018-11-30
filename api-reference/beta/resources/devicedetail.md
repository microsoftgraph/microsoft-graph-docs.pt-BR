---
title: tipo de recurso de deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para assinar. Inclui informações como o navegador do dispositivo e informações do sistema operacional, se o dispositivo for Azure AD gerenciado.
ms.openlocfilehash: d7c1830ee5c99fc139a937fcee3896e2a9926592
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034137"
---
# <a name="devicedetail-resource-type"></a>tipo de recurso de deviceDetail
Indica os detalhes do dispositivo associados a um dispositivo usado para assinar. Inclui informações como o navegador do dispositivo e informações do sistema operacional, se o dispositivo for Azure AD gerenciado.



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Navegador|String|Indica as informações do navegador dos usados para entrar no serviço.|
|deviceId|Cadeia de caracteres|Refere-se o UniqueID do dispositivo usado para entrar no serviço.|
|displayName|String|Refere-se com o nome do dispositivo usado para entrar no serviço.|
|isCompliant|Booliano|Indica se o dispositivo é compatível com ou não.|
|isManaged|Booliano|Indica se o dispositivo é gerenciado ou não.|
|operatingSystem|String|Indica o nome do sistema operacional e versão usada para entrar no serviço.|
|trustType|String|Indica se o dispositivo conectado é integrado ao domínio local de trabalho associado, AzureAD ingressado, as informações. |

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