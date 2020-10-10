---
title: tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação de entrada de telefone sem senha do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ddf6a66abbf745a769a44cf323ebb245c31ecf60
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418205"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type"></a>tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de métodos de autenticação de entrada de telefone sem senha do Microsoft Authenticator. Métodos de autenticação as políticas definem definições de configuração e usuários ou grupos que estão habilitados para usar o método de autenticação.

> [!NOTE]
> Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta. Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Get](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md)|[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|Leia as propriedades e os relacionamentos de um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.|
|[Atualizar](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md)|[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|Atualiza as propriedades de um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.|
|[Excluir](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md)|Nenhum|Reverte o objeto passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration para sua configuração padrão.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de política de método de autenticação.|
|estado|authenticationMethodState|Os valores possíveis são: `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|includeTargets|coleção [passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md)|Uma coleção de usuários ou grupos que estão habilitados para usar o método de autenticação.|

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
