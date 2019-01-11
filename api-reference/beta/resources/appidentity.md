---
title: tipo de recurso de appIdentity
description: Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui o Id do aplicativo, nome, ID de entidade de serviço e Name. Este recurso é chamado pelo API directoryAudit
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855780"
---
# <a name="appidentity-resource-type"></a>tipo de recurso de appIdentity
Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui o Id do aplicativo, nome, ID de entidade de serviço e Name. Este recurso é chamado pelo [directoryAudit](../api/directoryaudit-get.md) API


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appId|Cadeia de caracteres|Refere-se o GUID exclusivo que representa a Id do aplicativo no Windows Azure Active Directory.|
|displayName|Cadeia de caracteres|Refere-se ao nome do aplicativo exibido no Portal do Windows Azure.|
|servicePrincipalId|Cadeia de caracteres|Refere-se o GUID exclusivo que indica o Id da entidade de serviço no Windows Azure Active Directory para o aplicativo correspondente.|
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
