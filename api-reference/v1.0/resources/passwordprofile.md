---
title: Tipo de recurso passwordProfile
description: Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade user é um objeto **passwordProfile**.
localization_priority: Priority
author: eketo-msft
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 7288d2f737c0e04be9919ba0b2412df2ba1ebda8c377e1c66a3d6a91992af858
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189398"
---
# <a name="passwordprofile-resource-type"></a>Tipo de recurso passwordProfile

Namespace: microsoft.graph

Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade [user](user.md) é um objeto **passwordProfile**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|forceChangePasswordNextSignIn|Booliano| `true` se o usuário precisar alterar sua senha no próximo logon; caso contrário, `false`. Se não for definido, o padrão é `false`. **OBSERVAÇÃO:**  Para locatários do Azure B2C, defina `false` e use políticas personalizadas e fluxos de usuário para forçar a redefinição de senha na primeira entrada. Confira [Forçar redefinição de senha no primeiro logon](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon).|
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
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>Confira também

[Atualizar o passwordProfile de um usuário](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password)
