---
title: tipo de recurso defaultUserRolePermissions
description: Contém determinadas permissões personalizáveis de função de usuário padrão.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f2b4fbc4b4a496905f8199b065ecd94e849365e
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581179"
---
# <a name="defaultuserrolepermissions-resource-type"></a>tipo de recurso defaultUserRolePermissions

Contém determinadas permissões personalizáveis de função de usuário padrão no Azure Active Directory (AD).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| allowedToCreateApps | Boolean | Indica se a função de usuário padrão pode criar aplicativos. |  
| allowedToCreateSecurityGroups | Boolean | Indica se a função de usuário padrão pode criar grupos de segurança. |  
| allowedToReadOtherUsers | Boolean | Indica se a função de usuário padrão pode ler outros usuários. |
|permissionGrantPoliciesAssigned|Conjunto de cadeias de caracteres|Indica se o consentimento do usuário para os aplicativos é permitido e, se for, qual permissão para conceder consentimento e qual política de consentimento de aplicativo (permissionGrantPolicy) governará a permissão para os usuários concederem o consentimento. O valor deve estar no formato `managePermissionGrantsForSelf.{id}` , onde `{id}` é a **ID** de uma [política de consentimento de aplicativo](/azure/active-directory/manage-apps/manage-app-consent-policies)interna ou personalizada. Uma lista vazia indica que o consentimento do usuário para os aplicativos está desabilitado. |

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
