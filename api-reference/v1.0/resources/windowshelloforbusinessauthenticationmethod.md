---
title: Tipo de recurso windowsHelloForBusinessAuthenticationMethod
description: Uma representação de uma instância Windows Hello para Empresas registrada em um usuário. Windows Hello for Business é um método de autenticação de login.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9381749d42a61a8704a54434cf233dea8ad69240538de0022157656f522f1292
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196464"
---
# <a name="windowshelloforbusinessauthenticationmethod-resource-type"></a>Tipo de recurso windowsHelloForBusinessAuthenticationMethod

Namespace: microsoft.graph

Uma representação de um Windows Hello de autenticação para Empresas registrado para um usuário. Windows Hello para Empresas é um método de autenticação de entrada para Windows dispositivos.

Herda de [authenticationMethod](../resources/authenticationmethod.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsHelloForBusinessAuthenticationMethods](../api/windowshelloforbusinessauthenticationmethod-list.md)|[coleção windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|Obter uma lista dos [objetos windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) e suas propriedades.|
|[Obter windowsHelloForBusinessAuthenticationMethod](../api/windowshelloforbusinessauthenticationmethod-get.md)|[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|Leia as propriedades e as relações de um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)|
|[Excluir windowsHelloForBusinessAuthenticationMethod](../api/windowshelloforbusinessauthenticationmethod-delete.md)|None|Exclui um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e a hora em que essa chave Windows Hello para Empresas foi registrada.|
|displayName|String|O nome do dispositivo no qual o Windows Hello for Business está registrado|
|id|Cadeia de caracteres|Um identificador exclusivo para esse método de autenticação. Herdado da [autenticaçãoMethod](../resources/authenticationmethod.md)|
|keyStrength|authenticationMethodKeyStrength|Chave forte dessa chave de Windows Hello para Empresas. Os valores possíveis são: `normal`, `weak`, `unknown`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|device|[device](../resources/device.md)|O dispositivo registrado no qual esta chave Windows Hello para Empresas reside.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "createdDateTime": "String",
  "keyStrength": {"@odata.type": "microsoft.graph.authenticationMethodKeyStrength"}
}
```
