---
title: tipo de recurso appIdentity
description: Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui ID do aplicativo, nome, ID da entidade de serviço e nome. Este recurso é chamado pela API directoryAudit
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 63cb9ed2fbbf9487af1e4d523a04defb7c78cb9e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974315"
---
# <a name="appidentity-resource-type"></a>tipo de recurso appIdentity
Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui ID do aplicativo, nome, ID da entidade de serviço e nome. Este recurso é chamado pela API [directoryAudit](../api/directoryaudit-get.md)


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appId|Cadeia de caracteres|Se refere a GUID exclusivo que representa o Id de aplicativo no Azure Active Directory.|
|displayName|String|Refere-se ao nome do aplicativo exibido no portal do Azure.|
|servicePrincipalName|String|Refere-se ao GUID exclusivo indicando a ID da entidade de serviço no Azure Active Directory para o aplicativo correspondente.|
|servicePrincipalName|Cadeia de caracteres|Refere-se ao nome da entidade de segurança do serviço é o nome do aplicativo no locatário. |

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
