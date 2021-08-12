---
title: Tipo de recurso delegatedPermissionClassification
description: Usado para especificar a classificação de uma permissão delegada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: a7842eb4efdd54f63743a786b0be28990dee609a27fa960bfa38ac2e476921ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146990"
---
# <a name="delegatedpermissionclassification-resource-type"></a>Tipo de recurso delegatedPermissionClassification

Namespace: microsoft.graph

Usado para especificar a classificação de uma permissão delegada.

As classificações de permissão delegadas podem ser usadas em combinação com as configurações de consentimento do usuário para escolher quais permissões um usuário tem permissão para consentir. Consulte [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| id | Cadeia de caracteres | Um identificador exclusivo para **a chave delegatedPermissionClassification.** Não anulável. Somente leitura. |
| classificação | permissionClassificationType | O valor de classificação que está sendo dado. Valor possível: `low` . O não tem suporte para `$filter`. |
| permissionId | Guid | O identificador exclusivo (**id**) da permissão delegada listada na coleção **oauth2PermissionScopes** [do servicePrincipal](servicePrincipal.md). Obrigatório durante a criação. O não tem suporte para `$filter`. |
| permissionName | Cadeia de caracteres | O valor da declaração (**valor**) da permissão delegada listada na coleção **oauth2PermissionScopes** do [servicePrincipal](servicePrincipal.md). O não tem suporte para `$filter`. |

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
