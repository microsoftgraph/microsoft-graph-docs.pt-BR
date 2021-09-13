---
title: Tipo de recurso basicAuthentication
description: Representa a configuração para o uso da autenticação básica em uma chamada de API.
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9749d179ffa33020b73747e46ed21add6eb9316d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019395"
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
