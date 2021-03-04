---
title: Tipo de recurso windowsHelloForBusinessAuthenticationMethod
description: Uma representação de uma instância do Windows Hello para Empresas registrada em um usuário. O Windows Hello para Empresas é um método de autenticação de login.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3ac3f2cd3aed11943a1ab233cfbb64b7a75b32d0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433100"
---
# <a name="windowshelloforbusinessauthenticationmethod-resource-type"></a>Tipo de recurso windowsHelloForBusinessAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação de um método de autenticação do Windows Hello para Empresas registrado para um usuário. O Windows Hello para Empresas é um método de autenticação de entrada para dispositivos Windows.

Herda de [authenticationMethod](../resources/authenticationmethod.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsHelloForBusinessAuthenticationMethods](../api/windowshelloforbusinessauthenticationmethod-list.md)|[coleção windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|Obter uma lista dos [objetos windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) e suas propriedades.|
|[Obter windowsHelloForBusinessAuthenticationMethod](../api/windowshelloforbusinessauthenticationmethod-get.md)|[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|Leia as propriedades e as relações de um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)|
|[Excluir windowsHelloForBusinessAuthenticationMethod](../api/windowshelloforbusinessauthenticationmethod-delete.md)|Nenhum(a)|Exclui um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e a hora em que essa chave do Windows Hello para Empresas foi registrada.|
|displayName|String|O nome do dispositivo no qual o Windows Hello para Empresas está registrado|
|id|String|Um identificador exclusivo para esse método de autenticação. Herdado da [autenticaçãoMethod](../resources/authenticationmethod.md)|
|keyStrength|authenticationMethodKeyStrength|Força fundamental dessa chave do Windows Hello para Empresas. Os valores possíveis são: `normal`, `weak`, `unknown`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|device|[device](../resources/device.md)|O dispositivo registrado no qual esta chave do Windows Hello para Empresas reside.|

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
