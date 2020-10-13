---
title: tipo de recurso delegatedPermissionClassification
description: Usado para especificar a classificação de uma permissão delegada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: f41ea807859b11982283b2a9743d6167e99dac66
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433517"
---
# <a name="delegatedpermissionclassification-resource-type"></a>tipo de recurso delegatedPermissionClassification

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para especificar a classificação de uma permissão delegada.

As classificações de permissão delegada podem ser usadas em combinação com as configurações de consentimento do usuário para escolher a quais permissões um usuário pode concordar. Confira [configurar como os usuários finais consentiam aos aplicativos](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) para saber mais sobre as classificações de permissão.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| id | String | Um identificador exclusivo para a chave **delegatedPermissionClassification** . Não anulável. Somente leitura. |
| classificação | permissionClassificationType | O valor de classificação que está sendo fornecido. Valor possível: `low` . O não tem suporte para `$filter`. |
| permissionid | Guid | O identificador exclusivo (**ID**) da permissão delegada listada na coleção **publishedPermissionScopes** do [servicePrincipalName](servicePrincipal.md). Obrigatório durante a criação. O não tem suporte para `$filter`. |
| permissionname | String | O valor de declaração (**valor**) para a permissão delegada listada na coleção **publishedPermissionScopes** do [servicePrincipalName](servicePrincipal.md). O não tem suporte para `$filter`. |

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
