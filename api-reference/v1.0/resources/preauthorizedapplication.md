---
title: Tipo de recurso preAuthorizedApplication
description: Lista os aplicativos cliente pré-autorizados
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 25632d22161a5fb422cb67786f26fdc7c645bd4f
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118421"
---
# <a name="preauthorizedapplication-resource-type"></a>Tipo de recurso preAuthorizedApplication

Namespace: microsoft.graph

Lista os aplicativos cliente que são pré-autorizados com as permissões especificadas para acessar as APIs desse aplicativo. Os usuários não precisam consentir com nenhum aplicativo pré-autorizado (para as permissões especificadas). No entanto, quaisquer permissões adicionais não listadas em preAuthorizedApplications (solicitadas por meio de consentimento incremental, por exemplo) exigirão o consentimento do usuário.

Em alguns casos raros, um identificador `delegatedPermissionIds` listado na propriedade pode realmente identificar uma função de [aplicativo (](approle.md) `appRoles` da propriedade da entidade de serviço), `appId` indicando que o aplicativo cliente identificado pela propriedade foi pré-autorizado para essa função de aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|appId|String| O identificador exclusivo do aplicativo. |
|delegatedPermissionIds|Coleção de cadeias de caracteres| O identificador exclusivo para [o oauth2PermissionScopes](permissionscope.md) que o aplicativo requer. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "delegatedPermissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

