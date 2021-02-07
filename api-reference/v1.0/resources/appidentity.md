---
title: Tipo de recurso appIdentity
description: Indica a identidade do aplicativo que realizou a ação ou foi alterado. Inclui id do aplicativo, nome, ID da entidade de serviço e nome. Esse recurso é chamado pela API directoryAudit
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d0ba66e962f70a854fd028305b1e31c140ad1fe8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134992"
---
# <a name="appidentity-resource-type"></a>Tipo de recurso appIdentity

Namespace: microsoft.graph

Indica a identidade do aplicativo que realizou a ação ou foi alterado. Inclui a ID do aplicativo, o nome e a ID da entidade de serviço e o nome. Esse recurso é usado pela [operação Get directoryAudit.](../api/directoryaudit-get.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appId|Cadeia de caracteres|Se refere a GUID exclusivo que representa o Id de aplicativo no Azure Active Directory.|
|displayName|String|Refere-se ao Nome do Aplicativo exibido no Portal do Azure.|
|servicePrincipalId|String|Refere-se ao GUID exclusivo que indica a ID da entidade de serviço no Azure Active Directory para o aplicativo correspondente.|
|servicePrincipalName|Cadeia de caracteres|Refere-se ao nome da entidade de serviço é o nome do aplicativo no locatário. |

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

