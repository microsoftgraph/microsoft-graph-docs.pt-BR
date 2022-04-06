---
title: tipo de recurso de autenticação
description: Expõe relações que representam os métodos de autenticação suportados pelo Azure AD e que podem ser configurados para os usuários.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c098cc1b813a3805c1afc3956d93b6a416aa239
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510713"
---
# <a name="authentication-resource-type"></a>tipo de recurso de autenticação

Namespace: microsoft.graph

Expõe relações que representam os métodos de autenticação suportados pelo Azure AD e que podem ser configurados para os usuários.

Herda de [entidade](entity.md).

## <a name="methods"></a>Methods

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|fido2Methods|[coleção fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Representa as chaves de segurança FIDO2 registradas para um usuário para autenticação.|
|métodos|[Coleção authenticationMethod](../resources/authenticationmethod.md)| Representa todos os métodos de autenticação registrados para um usuário.|
|microsoftAuthenticatorMethods|[coleção microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)| Os detalhes do aplicativo Microsoft Authenticator registrado para um usuário para autenticação. |
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

