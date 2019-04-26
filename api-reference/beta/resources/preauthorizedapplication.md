---
title: tipo de recurso Preauthorizedapplication e
description: Representa um aplicativo e permissões solicitadas para o consentimento implícito. Requer um administrador para ter fornecido o consentimento para o aplicativo. o preAuthorizedApplications não exige que o usuário concorde com as permissões solicitadas. As permissões listadas no preAuthorizedApplications não exigem o consentimento do usuário. No enTanto, as permissões adicionais solicitadas não listadas no preAuthorizedApplications exigem o consentimento do usuário.
localization_priority: Normal
ms.openlocfilehash: f74ac0883c883bfbb2cb93c2da58e9fd8419dadd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344213"
---
# <a name="preauthorizedapplication-resource-type"></a>tipo de recurso Preauthorizedapplication e

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um aplicativo e permissões solicitadas para o consentimento implícito. Requer um administrador para ter fornecido o consentimento para o aplicativo. o preAuthorizedApplications não exige que o usuário concorde com as permissões solicitadas. As permissões listadas no preAuthorizedApplications não exigem o consentimento do usuário. No enTanto, as permissões adicionais solicitadas não listadas no preAuthorizedApplications exigem o consentimento do usuário.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|appId|String| O identificador exclusivo do aplicativo. |
|permissionIds|Coleção String| O identificador exclusivo do [publishedPermissionScope](permissionscope.md) ou do [appRole](approle.md) que o aplicativo exige. |

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
