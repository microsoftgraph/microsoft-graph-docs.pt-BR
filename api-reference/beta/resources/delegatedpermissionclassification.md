---
title: Tipo de recurso delegatedPermissionClassification
description: Usado para especificar a classificação de uma permissão delegada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 4a567696d2adf0cd2a53cc2eb4d193ec1e1c2855
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133634"
---
# <a name="delegatedpermissionclassification-resource-type"></a>Tipo de recurso delegatedPermissionClassification

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para especificar a classificação de uma permissão delegada.

As classificações de permissão delegada podem ser usadas em combinação com as configurações de consentimento do usuário para escolher quais permissões um usuário tem permissão para consentir. Consulte [Configurar como os usuários finais permitem que os aplicativos](/azure/active-directory/manage-apps/configure-user-consent) aprendam mais sobre classificações de permissão.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| id | String | Um identificador exclusivo para a **chave delegatedPermissionClassification.** Não anulável. Somente leitura. |
| classificação | permissionClassificationType | O valor de classificação sendo dado. Valor possível: `low` . O não tem suporte para `$filter`. |
| permissionId | Guid | O identificador exclusivo (**id**) para a permissão delegada listada na **coleção publishedPermissionScopes** do [servicePrincipal](servicePrincipal.md). Obrigatório durante a criação. O não tem suporte para `$filter`. |
| permissionName | String | O valor da declaração (**valor**) para a permissão delegada listada na **coleção publishedPermissionScopes** do [servicePrincipal](servicePrincipal.md). O não tem suporte para `$filter`. |

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

