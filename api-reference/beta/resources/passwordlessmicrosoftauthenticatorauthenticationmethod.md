---
title: passwordlessMicrosoftAuthenticatorAuthentication Tipo de recursoMethod
description: Uma representação de um método de Login de Telefone Sem Senha do Microsoft Authenticator registrado para um usuário.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0949a92d0adbcfdd53164b550b6d8f8bc07444eb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444074"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethod-resource-type-deprecated"></a>passwordlessMicrosoftAuthenticatorAuthentication Tipo de recursoMethod (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação de um método de Login de Telefone Sem Senha do Microsoft Authenticator registrado para um usuário.

> [!CAUTION]
> A API do método de login sem senha do Microsoft Authenticator Phone está preterida e interromperá o retorno dos resultados em 31 de dezembro de 2020. Use o novo [Método de Autenticação do Autenticador microsoft](../resources/microsoftAuthenticatorAuthenticationMethod.md).


## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md) (preterido)|[coleção passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|Recupere uma lista dos objetosMicrosoftAuthenticatorAuthenticatorAuthenticationMethod de um usuário e suas propriedades.|
|[Get](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md) (preterido)|[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|Leia as propriedades e as relações do objetoMicrosoftAuthenticatorAuthenticationMethod de um usuário.|
|[Excluir](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md) (preterido)|Nenhum(a)|Exclui o objetoMicrosoftAuthenticatorAuthenticationMethod de um usuário.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do método de autenticação.|
|displayName|String|O nome de exibição do dispositivo móvel conforme dado pelo usuário.|
|creationDateTime|DateTimeOffset|O timestamp quando esse método foi registrado para o usuário.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)"
}
```

