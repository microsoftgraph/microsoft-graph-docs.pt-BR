---
title: Tipo de recurso defaultUserRolePermissions
description: Contém determinadas permissões personalizáveis da função de usuário padrão.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0e89f175a62615efe172646613897222a9ae75fa
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137554"
---
# <a name="defaultuserrolepermissions-resource-type"></a>Tipo de recurso defaultUserRolePermissions

Contém determinadas permissões personalizáveis da função de usuário padrão no Azure Active Directory (AD).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| allowedToCreateApps | Booliano | Indica se a função de usuário padrão pode criar aplicativos. |  
| allowedToCreateSecurityGroups | Booliano | Indica se a função de usuário padrão pode criar grupos de segurança. |  
| allowedToReadOtherUsers | Booliano | Indica se a função de usuário padrão pode ler outros usuários. |
|permissionGrantPoliciesAssigned|String collection|Indica se o consentimento do usuário para aplicativos é permitido e, se for, qual permissão para conceder consentimento e qual política de consentimento do aplicativo (permissionGrantPolicy) regem a permissão para que os usuários concedam consentimento. Value should be in the format `managePermissionGrantsForSelf.{id}` , where is the `{id}` **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies). Uma lista vazia indica que o consentimento do usuário para aplicativos está desabilitado. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultUserRolePermissions"
}-->

```json
{
  "allowedToCreateApps": true,
  "allowedToCreateSecurityGroups": true,
  "allowedToReadOtherUsers": true,
  "permissionGrantPoliciesAssigned": ["String"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "defaultUserRolePermissions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
