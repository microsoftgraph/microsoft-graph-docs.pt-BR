---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethod
description: Uma representação do aplicativo Microsoft Authenticator registrado a um usuário. O Microsoft Authenticator é um método de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aeb2d1d7b111c9424da2f927dbaf3030a356c6b6
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796715"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a>Tipo de recurso microsoftAuthenticatorAuthenticationMethod

Namespace: microsoft.graph

Uma representação do aplicativo Microsoft Authenticator registrado a um usuário. O Microsoft Authenticator é um método de autenticação.

Herda de [authenticationMethod](../resources/authenticationmethod.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftAuthenticatorAuthenticationMethods](../api/microsoftauthenticatorauthenticationmethod-list.md)|[Coleção microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)|Obter uma lista dos [objetos microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) e suas propriedades.|
|[Obter microsoftAuthenticatorAuthenticationMethod](../api/microsoftauthenticatorauthenticationmethod-get.md)|[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)|Leia as propriedades e os relacionamentos de um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)|
|[Excluir microsoftAuthenticatorAuthenticationMethod](../api/microsoftauthenticatorauthenticationmethod-delete.md)|Nenhum|Exclui um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e a hora em que esse aplicativo foi registrado. Essa propriedade será nula se o dispositivo não estiver registrado para entrada por telefone sem senha.|
|displayName|Cadeia de caracteres|O nome do dispositivo no qual esse aplicativo está registrado.|
|id|Cadeia de caracteres|Um identificador exclusivo para esse método de autenticação. Herdado de [authenticationMethod](../resources/authenticationmethod.md)|
|deviceTag|String|Marcas que contêm metadados do aplicativo.|
|phoneAppVersion|Cadeia de caracteres|Versão numérica desta instância do aplicativo Autenticador.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|device|[device](../resources/device.md)|O dispositivo registrado no qual o Microsoft Authenticator reside. Essa propriedade será nula se o dispositivo não estiver registrado para entrada por telefone sem senha.|

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
