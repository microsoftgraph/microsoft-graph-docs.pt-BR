---
title: tipo de recurso Preauthorizedapplication e
description: Lista os aplicativos cliente pré autorizados
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: fdc6b9692076040a4495074456f1b847e3af3c69
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037245"
---
# <a name="preauthorizedapplication-resource-type"></a>tipo de recurso Preauthorizedapplication e

Namespace: microsoft.graph

Lista os aplicativos clientes que são previamente autorizados com as permissões especificadas para acessar as APIs desse aplicativo. Os usuários não precisam ser consentidos em qualquer aplicativo pré autorizado (para as permissões especificadas). No entanto, qualquer permissão adicional que não esteja listada no preAuthorizedApplications (solicitado por meio de consentimento incremental, por exemplo) exigirá o consentimento do usuário.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|appId|String| O identificador exclusivo do aplicativo. |
|delegatedPermissionIds|Coleção de cadeias de caracteres| O identificador exclusivo para o [oauth2PermissionScopes](permissionscope.md) que o aplicativo exige. |

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

