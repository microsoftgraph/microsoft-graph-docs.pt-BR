---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodConfiguration
description: Representa uma Microsoft Authenticator de métodos de autenticação.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ebe91061bedad1a21e0b4c6a5d388f875f8b7388
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067098"
---
# <a name="microsoftauthenticatorauthenticationmethodconfiguration-resource-type"></a>Tipo de recurso microsoftAuthenticatorAuthenticationMethodConfiguration
Namespace: microsoft.graph

Representa uma Microsoft Authenticator de métodos de autenticação. As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Get](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md)|[microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|Leia as propriedades e as relações de um objeto microsoftAuthenticatorAuthenticationMethodConfiguration.|
|[Atualizar](../api/microsoftauthenticatorauthenticationmethodconfiguration-update.md)|[microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|Atualize as propriedades de um objeto microsoftAuthenticatorAuthenticationMethodConfiguration.|
|[Delete](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md)|None|Reverte o objeto microsoftAuthenticatorAuthenticationMethodConfiguration para sua configuração padrão.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de política do método de autenticação.|
|state|authenticationMethodState|Os valores possíveis são: `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|includeTargets|[coleção microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md)|Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

