---
title: Tipo de recurso passwordProfile
description: Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade user é um objeto **passwordProfile**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: eketo-msft
ms.openlocfilehash: 7c0f31310227753caf3949a32046f067b4117770
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030863"
---
# <a name="passwordprofile-resource-type"></a>Tipo de recurso passwordProfile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade [user](user.md) é um objeto **passwordProfile**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|forceChangePasswordNextSignIn|Booliano|  `true` se o usuário precisar alterar sua senha no próximo logon; caso contrário, `false`. Se não estiver definido, o padrão será `false`. **OBSERVAÇÃO:**  Para locatários do Azure B2C, defina para e use políticas personalizadas e fluxos de usuários para forçar a redefinição de senha `false` ao entrar primeiro. Confira [Forçar a redefinição de senha no primeiro logon](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon). |
|forceChangePasswordNextSignInWithMfa|Booliano| Se `true`, na próxima conexão, o usuário deverá executar uma autenticação multifator (MFA) antes de ser forçado a alterar sua senha. O comportamento é idêntico a **forceChangePasswordNextSignIn**, exceto pelo fato de que o usuário deve primeiro executar uma autenticação multifator antes da alteração da senha. Após a alteração da senha, esta propriedade será redefinida automaticamente para `false`. Se não estiver definido, o padrão será `false`. |
|password|String|A senha do usuário. Essa propriedade é necessária ao criar um usuário. Pode ser atualizada, mas o usuário precisará alterar a senha no próximo login. A senha deve atender a requisitos mínimos, conforme especificado pelo a propriedade **passwordPolicies** do usuário. Por padrão, é necessária uma senha forte.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "forceChangePasswordNextSignInWithMfa": false,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


