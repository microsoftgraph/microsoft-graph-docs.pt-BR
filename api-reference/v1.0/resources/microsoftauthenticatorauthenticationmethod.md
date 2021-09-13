---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethod
description: Uma representação do aplicativo Microsoft Authenticator registrado para um usuário. Microsoft Authenticator é um método de autenticação.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ea3614af67720c9c35a641a3f6729eabf98d5dd8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134497"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a>Tipo de recurso microsoftAuthenticatorAuthenticationMethod

Namespace: microsoft.graph

Uma representação do aplicativo Microsoft Authenticator registrado para um usuário. Microsoft Authenticator é um método de autenticação.

Herda de [authenticationMethod](../resources/authenticationmethod.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftAuthenticatorAuthenticationMethods](../api/microsoftauthenticatorauthenticationmethod-list.md)|[coleção microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)|Obter uma lista dos [objetos microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) e suas propriedades.|
|[Obter microsoftAuthenticatorAuthenticationMethod](../api/microsoftauthenticatorauthenticationmethod-get.md)|[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)|Leia as propriedades e as relações de um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)|
|[Excluir microsoftAuthenticatorAuthenticationMethod](../api/microsoftauthenticatorauthenticationmethod-delete.md)|Nenhum(a)|Exclui um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e a hora em que esse aplicativo foi registrado. Essa propriedade será nula se o dispositivo não estiver registrado para entrada sem senha Telefone Entrada.|
|displayName|Cadeia de caracteres|O nome do dispositivo no qual esse aplicativo está registrado.|
|id|String|Um identificador exclusivo para esse método de autenticação. Herdado da [autenticaçãoMethod](../resources/authenticationmethod.md)|
|deviceTag|String|Marcas que contêm metadados de aplicativo.|
|phoneAppVersion|String|Versão numérica dessa instância do Authenticator app.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|device|[device](../resources/device.md)|O dispositivo registrado no qual Microsoft Authenticator reside. Essa propriedade será nula se o dispositivo não estiver registrado para entrada sem senha Telefone Entrada.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "deviceTag": "String",
  "phoneAppVersion": "String",
  "createdDateTime": "DateTimeOffset"
}
```
