---
title: Tipo de recurso preAuthorizedApplication
description: Lista os aplicativos cliente pré-autorizados
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 40fcfc642444be507fbd8e8a85f0052732293cb3
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118533"
---
# <a name="preauthorizedapplication-resource-type"></a>Tipo de recurso preAuthorizedApplication

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Lista os aplicativos cliente que são pré-autorizados com as permissões delegadas especificadas para acessar as APIs desse aplicativo. Os usuários não precisam consentir com nenhum aplicativo pré-autorizado (para as permissões especificadas). No entanto, quaisquer permissões adicionais não listadas em preAuthorizedApplications (solicitadas por meio de consentimento incremental, por exemplo) exigirão o consentimento do usuário.

Em alguns casos raros, um identificador `permissionIds` listado na propriedade pode se [referir a uma](approle.md) função de aplicativo ( `appRoles` da propriedade da entidade de serviço), `appId` indicando que o aplicativo cliente identificado pela propriedade foi pré-autorizado para essa função de aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|appId|Cadeia de caracteres| O identificador exclusivo do aplicativo cliente. |
|permissionIds|Coleção de cadeias de caracteres| O identificador exclusivo para os [escopos que](permissionscope.md) o aplicativo cliente recebe. |

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

