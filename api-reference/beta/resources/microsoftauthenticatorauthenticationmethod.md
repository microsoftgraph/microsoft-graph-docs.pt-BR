---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethod
description: Uma representação do aplicativo Microsoft Authenticator registrado para um usuário. Microsoft Authenticator é um método de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 07b5c2d776eb7867ffd3b0c847ead72e85bb6229
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298746"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a>Tipo de recurso microsoftAuthenticatorAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|id|Cadeia de caracteres|Um identificador exclusivo para esse método de autenticação. Herdado da [autenticaçãoMethod](../resources/authenticationmethod.md)|
|deviceTag|String|Marcas que contêm metadados de aplicativo.|
|phoneAppVersion|Cadeia de caracteres|Versão numérica dessa instância do Authenticator app.|

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
