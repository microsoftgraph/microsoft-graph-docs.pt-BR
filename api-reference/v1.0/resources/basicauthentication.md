---
title: Tipo de recurso basicAuthentication
description: Representa a configuração para o uso da autenticação básica em uma chamada de API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9bb61e297a6a668631da654383e13ee1dbf8ef79
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882381"
---
# <a name="basicauthentication-resource-type"></a>Tipo de recurso basicAuthentication

Namespace: microsoft.graph

Representa a configuração para o uso da autenticação HTTP Basic, que envolve um nome de usuário e uma senha, em uma chamada de API. O nome de usuário e a senha são enviados como o header de Autorização como onde está a versão codificada `Basic {value}` `value` base 64 de nome de usuário:senha.

Herda de [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|username|Cadeia de caracteres| O nome de usuário. |
|password|String| A senha. Ele não é retornado nas respostas. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.basicAuthentication"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.basicAuthentication",
  "password": "String",
  "username": "String"
}
```
