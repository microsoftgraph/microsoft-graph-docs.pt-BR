---
title: Tipo de recurso delegatedPermissionClassification
description: Usado para especificar a classificação de uma permissão delegada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: ff9f4ca394e2065c69fd7cd08a19d60817fc4f99
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761755"
---
# <a name="delegatedpermissionclassification-resource-type"></a>Tipo de recurso delegatedPermissionClassification

Namespace: microsoft.graph

Usado para especificar a classificação de uma permissão delegada.

As classificações de permissão delegadas podem ser usadas em combinação com as configurações de consentimento do usuário para escolher quais permissões um usuário tem permissão para consentir. Consulte [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| id | String | Um identificador exclusivo para **a chave delegatedPermissionClassification.** Não anulável. Somente leitura. |
| classificação | permissionClassificationType | O valor de classificação que está sendo dado. Valor possível: `low` . O não tem suporte para `$filter`. |
| permissionId | Guid | O identificador exclusivo (**id**) da permissão delegada listada na coleção **oauth2PermissionScopes** [do servicePrincipal](servicePrincipal.md). Obrigatório durante a criação. O não tem suporte para `$filter`. |
| permissionName | String | O valor da declaração (**valor**) da permissão delegada listada na coleção **oauth2PermissionScopes** do [servicePrincipal](servicePrincipal.md). O não tem suporte para `$filter`. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
}-->

```json
{
  "id": "string (identifier)",
  "classification": "low",
  "permissionId": "string",
  "permissionName": "string"
}
```
