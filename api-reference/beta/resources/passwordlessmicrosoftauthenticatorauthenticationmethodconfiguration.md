---
title: Tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação de Login de Telefone sem Senha do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e27424264293d87775937c7893546ec321728b4a
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872279"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type-deprecated"></a>Tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de métodos de autenticação de Login de Telefone sem Senha do Microsoft Authenticator. As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.

> [!CAUTION]
> A API do método de autenticação de autenticação de telefone sem senha do Microsoft Authenticator foi preterida e parou de retornar resultados em 31 de dezembro de 2020. Use a nova política [de método de autenticação do Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md) (preterido)|[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|Leia as propriedades e os relacionamentos de um objetoMicrosoftAuthenticatorAuthenticationMethodConfiguration sem senha.|
|[Atualização](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md) (preterido) |[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|Atualizar as propriedades de um objetoMicrosoftAuthenticatorAuthenticationMethodConfiguration sem senha.|
|[Excluir](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md) (preterido)|Nenhum|Reverte o objetoMicrosoftAuthenticatorAuthenticationMethodConfiguration sem senha para sua configuração padrão.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de política do método de autenticação.|
|state|authenticationMethodState|Os valores possíveis são: `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|includeTargets|[Coleção passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md)|Uma coleção de usuários ou grupos que estão habilitados para usar o método de autenticação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
