---
title: tipo de recurso delegatedPermissionClassification
description: Usado para especificar a classificação de uma permissão delegada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 7d5926bff0d7096080aa22fae49d0ed15c7d1fcd
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377174"
---
# <a name="delegatedpermissionclassification-resource-type"></a>tipo de recurso delegatedPermissionClassification

Namespace: microsoft.graph

Usado para especificar a classificação de uma permissão delegada.

As classificações de permissão delegada podem ser usadas em combinação com as configurações de consentimento do usuário para escolher a quais permissões um usuário pode concordar. Confira [configurar como os usuários finais consentiam aos aplicativos](/azure/active-directory/manage-apps/configure-user-consent) para saber mais sobre as classificações de permissão.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| id | String | Um identificador exclusivo para a chave **delegatedPermissionClassification** . Não anulável. Somente leitura. |
| classificação | permissionClassificationType | O valor de classificação que está sendo fornecido. Valor possível: `low` . O não tem suporte para `$filter`. |
| permissionid | Guid | O identificador exclusivo (**ID**) da permissão delegada listada na coleção **oauth2PermissionScopes** do [servicePrincipalName](servicePrincipal.md). Obrigatório durante a criação. O não tem suporte para `$filter`. |
| permissionname | Cadeia de Caracteres | O valor de declaração (**valor**) para a permissão delegada listada na coleção **oauth2PermissionScopes** do [servicePrincipalName](servicePrincipal.md). O não tem suporte para `$filter`. |

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
