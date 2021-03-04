---
title: Tipo de recurso fido2AuthenticationMethod
description: Uma representação de uma chave de segurança FIDO2 registrada em um usuário. FIDO2 é um método de autenticação de login.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a6cfed32f6e657608b70c799d348c6818e56a8c7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440322"
---
# <a name="fido2authenticationmethod-resource-type"></a>Tipo de recurso fido2AuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação de uma chave de segurança FIDO2 registrada em um usuário. FIDO2 é um método de autenticação de login.


## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List](../api/fido2authenticationmethod-list.md)|[coleção fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Recupere uma lista dos objetos fido2AuthenticationMethod de um usuário e suas propriedades.|
|[Get](../api/fido2authenticationmethod-get.md)|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Leia as propriedades e as relações do objeto fido2AuthenticationMethod de um usuário.|
|[Delete](../api/fido2authenticationmethod-delete.md)|Nenhum(a)|Exclui o objeto fido2AuthenticationMethod de um usuário.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do método de autenticação.|
|displayName|String|O nome de exibição da chave conforme dado pelo usuário.|
|creationDateTime|DateTimeOffset|O timestamp quando essa chave foi registrada para o usuário.|
|aaGuid|String|GUID de Atestado de Autenticador, um identificador que indica o tipo (por exemplo, make e model) do autenticador.|
|modelo|String|O modelo atribuído pelo fabricante da chave de segurança FIDO2.|
|attestationCertificates|Coleção de cadeias de caracteres|Os certificados de atestado anexados a essa chave de segurança.|
|attestationLevel|attestationLevel|O nível de atestado dessa chave de segurança FIDO2. Os valores possíveis são: `attested` , ou `notAttested` .|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fido2AuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)",
  "aaGuid": "String",
  "model": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String"
}
```

