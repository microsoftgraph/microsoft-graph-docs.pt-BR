---
title: Tipo de recurso delegatedPermissionClassification
description: Usado para especificar a classificação de uma permissão delegada.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 72cc4630ba8f28fe0d76722178edcdd3ffed5943
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854640"
---
# <a name="delegatedpermissionclassification-resource-type"></a>Tipo de recurso delegatedPermissionClassification

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para especificar a classificação de uma permissão delegada.

As classificações de permissão delegadas podem ser usadas em combinação com as configurações de consentimento do usuário para escolher quais permissões um usuário tem permissão para consentir. Consulte [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| id | String | Um identificador exclusivo para **a chave delegatedPermissionClassification** . Não anulável. Somente leitura. |
| classificação | permissionClassificationType | O valor de classificação que está sendo dado. Valor possível: `low`. O não tem suporte para `$filter`. |
| permissionId | GUID | O identificador exclusivo (**id**) da permissão delegada listada na coleção **publishedPermissionScopes** do [servicePrincipal](servicePrincipal.md). Obrigatório durante a criação. O não tem suporte para `$filter`. |
| permissionName | String | O valor da declaração (**valor**) da permissão delegada listada na coleção **publishedPermissionScopes** do [servicePrincipal](servicePrincipal.md). O não tem suporte para `$filter`. |

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

