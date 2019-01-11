---
title: tipo de recurso de preAuthorizedApplication
description: Representa um aplicativo e as permissões solicitadas para consentimento implícito. Requer um administrador tenha fornecido a consentimento para o aplicativo. preAuthorizedApplications não exigem o usuário concorda com as permissões solicitadas. Permissões listadas na preAuthorizedApplications não exigem consentimento do usuário. No entanto, qualquer permissões solicitadas adicionais não listados no preAuthorizedApplications exigem o consentimento do usuário.
localization_priority: Normal
ms.openlocfilehash: fa26b8046b81db70300b8ff40abcbd2b84f3f0c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832792"
---
# <a name="preauthorizedapplication-resource-type"></a>tipo de recurso de preAuthorizedApplication

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um aplicativo e as permissões solicitadas para consentimento implícito. Requer um administrador tenha fornecido a consentimento para o aplicativo. preAuthorizedApplications não exigem o usuário concorda com as permissões solicitadas. Permissões listadas na preAuthorizedApplications não exigem consentimento do usuário. No entanto, qualquer permissões solicitadas adicionais não listados no preAuthorizedApplications exigem o consentimento do usuário.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|appId|Cadeia de caracteres| O identificador exclusivo para o aplicativo. |
|permissionIds|String collection| O identificador exclusivo para o [publishedPermissionScope](permissionscope.md) ou [appRole](approle.md) o aplicativo requer. |

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
<!-- {
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
