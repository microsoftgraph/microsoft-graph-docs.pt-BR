---
title: Tipo de recurso emailAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação OTP de email
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 06b7159cd14df1ee5826f4d11275e44f7819008a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231819"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a>Tipo de recurso emailAuthenticationMethodConfiguration

Namespace: microsoft.graph

Representa a política de métodos de autenticação OTP de email desse locatário. As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação. O OTP de email pode ser usado pelos usuários nativos da nuvem do locatário para redefinição de senha de autoatendados ou por usuários externos para autenticação durante o resgate de convites e a inscrição de autoatendida para aplicativos específicos em fluxos de usuário.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-get.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|Leia as propriedades e as relações de um objeto emailAuthenticationMethodConfiguration.|
|[Atualizar emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-update.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|Atualize as propriedades de um objeto emailAuthenticationMethodConfiguration.|
|[Excluir emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-delete.md)|Nenhum|Exclui um objeto emailAuthenticationMethodConfiguration.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador de política do método de autenticação. Herdado [da autenticaçãoMethodConfiguration](../resources/authenticationmethodconfiguration.md).|
|state|authenticationMethodState|Indica se esse método de autenticação está habilitado ou não. Os valores possíveis são: `enabled` e `disabled`.|
|allowExternalIdToUseEmailOtp|externalEmailOtpState|Determina se o OTP de email pode ser usuável por usuários externos para autenticação. Os valores possíveis são: `default`, `enabled`, `disabled`, `unknownFutureValue`. Os locatários no estado que não utilizaram a visualização pública terão automaticamente o OTP de email habilitado a partir `default` de outubro de 2021.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|includeTargets|[coleção authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.|

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
