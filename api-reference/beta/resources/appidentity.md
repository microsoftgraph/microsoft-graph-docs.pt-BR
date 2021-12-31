---
title: Tipo de recurso appIdentity
description: Indica a identidade do aplicativo que realizou a ação ou foi alterado. Inclui ID do Aplicativo, Nome, ID da Entidade de Serviço e Nome. Esse recurso é chamado pela API directoryAudit
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: sureshja
ms.openlocfilehash: 7b1005b058508bdb128788836667c05dcc936dd6
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61646976"
---
# <a name="appidentity-resource-type"></a>Tipo de recurso appIdentity

Namespace: microsoft.graph

Indica a identidade do aplicativo que realizou a ação ou foi alterado. Esse recurso é chamado pela API [directoryAudit.](../api/directoryaudit-get.md)


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appId|Cadeia de caracteres|Se refere a GUID exclusivo que representa o Id de aplicativo no Azure Active Directory.|
|displayName|String|Refere-se ao Nome do Aplicativo exibido no Portal do Azure.|
|servicePrincipalId|String|Refere-se ao GUID exclusivo que indica a ID da Entidade de Serviço Azure Active Directory para o aplicativo correspondente.|
|servicePrincipalName|Cadeia de caracteres|Refere-se ao Nome da Entidade de Serviço é o nome do aplicativo no locatário. |

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


