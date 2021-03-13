---
title: Tipo de recurso basicAuthentication
description: Representa a configuração para o uso da autenticação básica em uma chamada de API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 396cadec8e1766bee662c51df8d7999ba6a0ba6c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761685"
---
# <a name="basicauthentication-resource-type"></a>Tipo de recurso basicAuthentication

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a configuração para o uso da autenticação HTTP Basic, que envolve um nome de usuário e uma senha, em uma chamada de API. O nome de usuário e a senha são enviados como o header de Autorização como onde está a versão codificada `Basic {value}` `value` base 64 de nome de usuário:senha.

Herda de [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|username|Cadeia de Caracteres| O nome de usuário. |
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
