---
title: Tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: Uma representação de um método de login de telefone sem senha do Microsoft Authenticator registrado para um usuário.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8815d84a8a85491399e97f7d10aa2e6cc1aeaf9d
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796546"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethod-resource-type-deprecated"></a>Tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethod (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação de um método de login de telefone sem senha do Microsoft Authenticator registrado para um usuário.

> [!CAUTION]
> A API do método de login de telefone sem senha do Microsoft Authenticator foi preterida e interromperá o retorno dos resultados em 31 de dezembro de 2020. Use o novo Método [de Autenticação do Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethod.md)


## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md) (preterida)|[Coleção passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|Recupere uma lista de objetosMicrosoftAuthenticatorAuthenticationMethod sem senha de um usuário e suas propriedades.|
|[Obter](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md) (preterido)|[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|Leia as propriedades e os relacionamentos do objetoMicrosoftAuthenticatorAuthenticationMethod sem senha de um usuário.|
|[Excluir](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md) (preterido)|Nenhum|Exclui um objetoMicrosoftAuthenticatorAuthenticationMethod sem senha de um usuário.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador do método de autenticação.|
|displayName|Cadeia de caracteres|O nome de exibição do dispositivo móvel conforme determinado pelo usuário.|
|creationDateTime|DateTimeOffset|O timestamp quando esse método foi registrado ao usuário.|


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

