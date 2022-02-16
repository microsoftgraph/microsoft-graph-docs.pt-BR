---
title: Tipo de recurso delegatedPermissionClassification
description: Usado para especificar a classificação de uma permissão delegada.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: faa6afc6c7f72efc73189d373c4f9223b558ecc7
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854348"
---
# <a name="delegatedpermissionclassification-resource-type"></a>Tipo de recurso delegatedPermissionClassification

Namespace: microsoft.graph

Usado para especificar a classificação de uma permissão delegada.

As classificações de permissão delegadas podem ser usadas em combinação com as configurações de consentimento do usuário para escolher quais permissões um usuário tem permissão para consentir. Consulte [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| id | String | Um identificador exclusivo para **a chave delegatedPermissionClassification** . Não anulável. Somente leitura. |
| classificação | permissionClassificationType | O valor de classificação que está sendo dado. Valor possível: `low`. O não tem suporte para `$filter`. |
| permissionId | String | O identificador exclusivo (**id**) da permissão delegada listada na coleção **oauth2PermissionScopes** do [servicePrincipal](servicePrincipal.md). Obrigatório durante a criação. O não tem suporte para `$filter`. |
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
  "id": "String (identifier)",
  "classification": "low",
  "permissionId": "String",
  "permissionName": "String"
}
```
