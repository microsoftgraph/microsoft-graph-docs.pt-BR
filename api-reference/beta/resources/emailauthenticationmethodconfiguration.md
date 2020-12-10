---
title: tipo de recurso emailAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação OTP de email
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3e3e18973759d7f120dd0bd8e984c98568054960
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617107"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a>tipo de recurso emailAuthenticationMethodConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a política dos métodos de autenticação OTP de email do locatário. Métodos de autenticação as políticas definem definições de configuração e usuários ou grupos que estão habilitados para usar o método de autenticação. A OTP de email pode ser usada pelos usuários de nuvem nativa do locatário para redefinição de senha de autoatendimento ou por usuários externos para autenticação em algumas circunstâncias.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-get.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|Leia as propriedades e os relacionamentos de um objeto emailAuthenticationMethodConfiguration.|
|[Atualizar emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-update.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|Atualiza as propriedades de um objeto emailAuthenticationMethodConfiguration.|
|[Excluir emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-delete.md)|Nenhum|Exclui um objeto emailAuthenticationMethodConfiguration.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de política de método de autenticação. Herdado de [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md).|
|state|authenticationMethodState|Indica se este método de autenticação está habilitado ou não. Os valores possíveis são: `enabled` e `disabled`.|
|allowExternalIdToUseEmailOtp|externalEmailOtpState|Determina se a OTP de email pode ser usada por usuários externos para autenticação. Os valores possíveis são: `default`, `enabled`, `disabled`, `unknownFutureValue`. Os locatários no `default` estado que não usaram a visualização pública serão automaticamente habilitados para a OTP de email a partir de março de 2021.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|includeTargets|coleção [authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Uma coleção de usuários ou grupos que estão habilitados para usar o método de autenticação.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "allowExternalIdToUseEmailOtp": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
