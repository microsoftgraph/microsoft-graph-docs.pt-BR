---
title: Tipo de recurso b2cAuthenticationMethodsPolicy
description: Representa um método de autenticação de conta local registrado para um usuário configurado em um locatário Azure Active Directory (Azure AD) B2C.
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 74b18a2a0bc6d0ace2062f07d44eb175f7ad39e9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161758"
---
# <a name="b2cauthenticationmethodspolicy-resource-type"></a>Tipo de recurso b2cAuthenticationMethodsPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Azure Active Directory (Azure AD) B2C permite que os administradores de locatários escolham um mecanismo para permitir que os usuários finais se registrem por meio de contas locais. Contas locais são as contas em que o Azure AD faz a asserção de identidade, em oposição a um provedor de identidade federada, como Google ou Facebook, etc.

As contas locais no Azure AD B2C não seguem as configurações ou paradigmas do Azure AD. A política de métodos de autenticação do Azure AD não é usada ou aplicada pelo Azure AD B2C. O Azure AD B2C armazena essas configurações em uma política diferente, que é consumida pelos fluxos do usuário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter b2cAuthenticationMethodsPolicy](../api/b2cauthenticationmethodspolicy-get.md) | [b2cauthenticationmethodspolicy](b2cauthenticationmethodspolicy.md) | Leia as propriedades de um objeto **b2cAuthenticationMethodsPolicy**. |
| [Atualizar b2cAuthenticationMethodsPolicy](../api/b2cauthenticationmethodspolicy-update.md) | Nenhum | Atualize as propriedades de um objeto **b2cAuthenticationMethodsPolicy**. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|A id da política de métodos de autenticação do B2C. Esta é a chave e uma propriedade somente leitura.|
|isEmailPasswordAuthenticationEnabled|Booliano|O administrador de locatário pode configurar contas locais usando o email se o método de autenticação de email e senha estiver habilitado.|
|isUserNameAuthenticationEnabled|Booliano|O administrador de locatários pode configurar contas locais usando o nome de usuário se o método de autenticação do nome de usuário e senha estiver habilitado.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.b2cAuthenticationMethodsPolicy",
  "keyProperty": "id"
}-->

```json
{
    "id": "b2CAuthenticationMethodsPolicy",
    "isEmailPasswordAuthenticationEnabled": true,
    "isUserNameAuthenticationEnabled": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "b2cAuthenticationMethodsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
