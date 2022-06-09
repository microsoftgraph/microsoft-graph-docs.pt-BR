---
title: tipo de recurso de autenticação
description: Expõe relações que representam os métodos de autenticação compatíveis com o Azure AD e que podem ser configurados para os usuários.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 34a7877f8b88e319cfb4ff0e710b064f56365eae
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971375"
---
# <a name="authentication-resource-type"></a>tipo de recurso de autenticação

Namespace: microsoft.graph

Expõe relações que representam os métodos de autenticação compatíveis com o Azure AD e que podem ser configurados para os usuários.

Herda de [entidade](entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|fido2Methods|[Coleção fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Representa as chaves de segurança FIDO2 registradas para um usuário para autenticação.|
|Métodos|[Coleção authenticationMethod](../resources/authenticationmethod.md)| Representa todos os métodos de autenticação registrados para um usuário.|
|microsoftAuthenticatorMethods|[coleção microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)| Os detalhes do aplicativo Microsoft Authenticator registrados para um usuário para autenticação. |
|temporaryAccessPassMethods|[Coleção temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Representa uma Passagem de Acesso Temporária registrada para um usuário para autenticação por meio de senhas com tempo limitado.|
|windowsHelloForBusinessMethods|[coleção windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|Representa o método de autenticação do Windows Hello para Empresas registrado para um usuário para autenticação.|

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
