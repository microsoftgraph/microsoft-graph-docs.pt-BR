---
title: tipo de recurso appIdentity
description: Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui ID do aplicativo, nome, ID da entidade de serviço e nome. Este recurso é chamado pela API directoryAudit
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a1878aa01f2a6594f102647b6642eab6f301fa91
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988594"
---
# <a name="appidentity-resource-type"></a>tipo de recurso appIdentity

Namespace: microsoft.graph

Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui a ID de aplicativo, o nome e a ID e o nome da entidade de serviço. Este recurso é usado pela operação [Get directoryAudit](../api/directoryaudit-get.md) .

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

