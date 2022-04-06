---
title: tipo de recurso de autenticação
description: Expõe relações que representam os métodos de autenticação suportados pelo Azure AD e que podem ser configurados para os usuários.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7bf797abcaa2117e603cf7eec69d13d981c5f5ec
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510727"
---
# <a name="authentication-resource-type"></a>tipo de recurso de autenticação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Expõe relações que representam os métodos de autenticação suportados pelo Azure AD e que podem ser configurados para os usuários.

Herda de [entidade](entity.md).

## <a name="methods"></a>Methods

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|emailMethods|[Coleção emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Representa os endereços de email registrados para um usuário para autenticação. |
|fido2Methods|[coleção fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Representa as chaves de segurança FIDO2 registradas para um usuário para autenticação.|
|métodos|[Coleção authenticationMethod](../resources/authenticationmethod.md)| Representa todos os métodos de autenticação registrados para um usuário.|
|microsoftAuthenticatorMethods|[coleção microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)| Os detalhes do aplicativo Microsoft Authenticator registrado para um usuário para autenticação. |
|passwordlessMicrosoftAuthenticatorMethods|[coleção passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|Representa o Microsoft Authenticator métodos de Telefone de login registrados em um usuário para autenticação.|
|passwordMethods|[coleção passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md)|Representa os detalhes do método de autenticação de senha registrado em um usuário para autenticação.|
|phoneMethods|[Coleção phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)|Representa o telefone registrado para um usuário para autenticação. |
|temporaryAccessPassMethods|[coleção temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Representa um Passe de Acesso Temporário registrado para um usuário para autenticação por meio de senhas limitadas ao tempo.|
|windowsHelloForBusinessMethods|[coleção windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|Representa o Windows Hello para Empresas de autenticação registrado para um usuário para autenticação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authentication",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authentication"
}
```

