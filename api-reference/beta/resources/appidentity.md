---
title: tipo de recurso de appIdentity
description: Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui o Id do aplicativo, nome, ID de entidade de serviço e Name. Este recurso é chamado pelo API directoryAudit
ms.openlocfilehash: 6fcbe8dbb1e17139111c5f1fa9e8681cd1b996a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036960"
---
# <a name="appidentity-resource-type"></a>tipo de recurso de appIdentity
Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui o Id do aplicativo, nome, ID de entidade de serviço e Name. Este recurso é chamado pelo [directoryAudit](../api/directoryaudit-get.md) API


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appId|Cadeia de caracteres|Refere-se o GUID exclusivo que representa a Id do aplicativo no Windows Azure Active Directory.|
|displayName|String|Refere-se ao nome do aplicativo exibido no Portal do Windows Azure.|
|servicePrincipalId|String|Refere-se o GUID exclusivo que indica o Id da entidade de serviço no Windows Azure Active Directory para o aplicativo correspondente.|
|servicePrincipalName|Cadeia de caracteres|Refere-se para o nome de entidade de serviço é o nome do aplicativo no inquilino. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appIdentity"
}-->

```json
{
  "appId": "String",
  "displayName": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->