---
title: tipo de recurso Preauthorizedapplication e
description: Representa um aplicativo e permissões solicitadas para o consentimento implícito. Requer um administrador para ter fornecido o consentimento para o aplicativo. o preAuthorizedApplications não exige que o usuário concorde com as permissões solicitadas. As permissões listadas no preAuthorizedApplications não exigem o consentimento do usuário. No entanto, as permissões adicionais solicitadas não listadas no preAuthorizedApplications exigem o consentimento do usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7adaf4fe960b762b12f6b2cc8607e64c9813712e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965811"
---
# <a name="preauthorizedapplication-resource-type"></a>tipo de recurso Preauthorizedapplication e

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um aplicativo e permissões solicitadas para o consentimento implícito. Requer um administrador para ter fornecido o consentimento para o aplicativo. o preAuthorizedApplications não exige que o usuário concorde com as permissões solicitadas. As permissões listadas no preAuthorizedApplications não exigem o consentimento do usuário. No entanto, as permissões adicionais solicitadas não listadas no preAuthorizedApplications exigem o consentimento do usuário.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|appId|String| O identificador exclusivo do aplicativo. |
|permissionIds|Coleção de cadeias de caracteres| O identificador exclusivo do [publishedPermissionScope](permissionscope.md) ou do [appRole](approle.md) que o aplicativo exige. |

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
