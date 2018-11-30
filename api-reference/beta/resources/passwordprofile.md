---
title: Tipo de recurso passwordProfile
description: Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade user é um objeto **passwordProfile**.
ms.openlocfilehash: 71a91f0848ba8218d16a59c9e1f867d14e5cad9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040991"
---
# <a name="passwordprofile-resource-type"></a>Tipo de recurso passwordProfile

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade [user](user.md) é um objeto **passwordProfile**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|forceChangePasswordNextSignIn|Booliano| Se **verdadeiro**, na próxima tela de entrada, o usuário deve alterar sua senha. Após uma alteração de senha, essa propriedade será redefinida automaticamente como ***false**. Se não for definido, o padrão é **false**. |
|forceChangePasswordNextSignInWithMfa|Booliano| Se **verdadeiro**, na próxima tela de entrada, o usuário deve executar uma autenticação multifator (MFA) antes de serem é forçado a alterar sua senha. O comportamento é idêntico ao **forceChangePasswordNextSignIn** , exceto pelo fato do usuário é necessário para realizar primeiro uma autenticação multifator antes de alteração de senha. Após uma alteração de senha, esta propriedade será redefinida para **false**automaticamente. Se não for definido, o padrão é **false**. |
|password|String|A senha do usuário. Essa propriedade é necessária ao criar um usuário. Pode ser atualizada, mas o usuário precisará alterar a senha no próximo login. A senha deve atender a requisitos mínimos, conforme especificado pelo a propriedade **passwordPolicies** do usuário. Por padrão, é necessária uma senha forte.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordprofile"
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