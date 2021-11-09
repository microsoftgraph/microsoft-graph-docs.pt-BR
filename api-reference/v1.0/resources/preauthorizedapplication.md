---
title: Tipo de recurso preAuthorizedApplication
description: Lista os aplicativos cliente pré-autorizados
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 0f28c771f267324a25198edd66ac64ff7bcdaadd
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780538"
---
# <a name="preauthorizedapplication-resource-type"></a>Tipo de recurso preAuthorizedApplication

Namespace: microsoft.graph

Lista os aplicativos cliente pré-autorizados com as permissões especificadas para acessar as APIs desse aplicativo. Os usuários não precisam consentir com nenhum aplicativo pré-autorizado (para as permissões especificadas). No entanto, quaisquer permissões adicionais não listadas em preAuthorizedApplications (solicitadas por meio do consentimento incremental, por exemplo) exigirão o consentimento do usuário.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|appId|String| O identificador exclusivo do aplicativo. |
|permissionIds|Coleção de cadeias de caracteres| O identificador exclusivo para [o oauth2PermissionScopes](permissionscope.md) que o aplicativo requer. |

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
  "permissionIds": ["String"]
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

