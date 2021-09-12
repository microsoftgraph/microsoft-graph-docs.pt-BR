---
title: tipo de recurso defaultUserRolePermissions
description: Contém determinadas permissões personalizáveis da função de usuário padrão.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2e102061864c39fcba9354fce916cf57c43a88b6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59007226"
---
# <a name="defaultuserrolepermissions-resource-type"></a>tipo de recurso defaultUserRolePermissions

Contém determinadas permissões personalizáveis da função de usuário padrão no Azure Active Directory (AD).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| allowedToCreateApps | Booliano | Indica se a função de usuário padrão pode criar aplicativos. |  
| allowedToCreateSecurityGroups | Booliano | Indica se a função de usuário padrão pode criar grupos de segurança. |  
| allowedToReadOtherUsers | Boolean | Indica se a função de usuário padrão pode ler outros usuários. |
|permissionGrantPoliciesAssigned|Coleção String|Indica se o consentimento do usuário para aplicativos é permitido e, se for, qual permissão conceder consentimento e qual política de consentimento de aplicativo (permissionGrantPolicy) regem a permissão para que os usuários concedam consentimento. O valor deve estar no formato `managePermissionGrantsForSelf.{id}` , onde é a `{id}` **id** de uma política de consentimento de aplicativo interna ou [personalizada.](/azure/active-directory/manage-apps/manage-app-consent-policies) Uma lista vazia indica que o consentimento do usuário para aplicativos está desabilitado. |

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
