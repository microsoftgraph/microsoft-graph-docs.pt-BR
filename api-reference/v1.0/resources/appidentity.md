---
title: Tipo de recurso appIdentity
description: Indica a identidade do aplicativo que realizou a ação ou foi alterado. Inclui ID do Aplicativo, Nome, ID da Entidade de Serviço e Nome. Esse recurso é chamado pela API directoryAudit
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 0d9347ecf3571b89843c6e2b83454d6ae45b5b65405ba66914227a994abc0fb7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155208"
---
# <a name="appidentity-resource-type"></a>Tipo de recurso appIdentity

Namespace: microsoft.graph

Indica a identidade do aplicativo que realizou a ação ou foi alterado. Inclui a ID, o nome e o nome da entidade de serviço. Esse recurso é usado pela [operação Get directoryAudit.](../api/directoryaudit-get.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appId|Cadeia de caracteres|Se refere a GUID exclusivo que representa o Id de aplicativo no Azure Active Directory.|
|displayName|Cadeia de caracteres|Refere-se ao Nome do Aplicativo exibido no Portal do Azure.|
|servicePrincipalId|Cadeia de caracteres|Refere-se ao GUID exclusivo que indica a ID da Entidade de Serviço Azure Active Directory para o aplicativo correspondente.|
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

