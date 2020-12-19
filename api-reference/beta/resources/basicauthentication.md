---
title: tipo de recurso basicAuthentication
description: Representa a configuração para usar a autenticação básica em uma chamada de API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9de5fad9746e8562f51d1ddc8fcea350c41979ed
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720090"
---
# <a name="basicauthentication-resource-type"></a>tipo de recurso basicAuthentication

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a configuração para usar a autenticação básica HTTP, que envolve um nome de usuário e senha em uma chamada de API. O nome de usuário e a senha são enviados como o cabeçalho de autorização, como a `Basic {value}` `value` versão base 64 codificada de nome de usuário: senha.

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
