---
title: Tipo de recurso fido2AuthenticationMethod
description: Uma representação de uma chave de segurança FIDO2 registrada em um usuário. FIDO2 é um método de autenticação de login.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0c79a704d9a2aa899ffc2a3f4592f76a30d30126
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964621"
---
# <a name="fido2authenticationmethod-resource-type"></a>Tipo de recurso fido2AuthenticationMethod

Namespace: microsoft.graph

Uma representação de uma chave de segurança FIDO2 registrada em um usuário. FIDO2 é um método de autenticação de login.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List](../api/fido2authenticationmethod-list.md)|[coleção fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Recupere uma lista dos objetos fido2AuthenticationMethod de um usuário e suas propriedades.|
|[Get](../api/fido2authenticationmethod-get.md)|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Leia as propriedades e as relações do objeto fido2AuthenticationMethod de um usuário.|
|[Delete](../api/fido2authenticationmethod-delete.md)|Nenhum|Exclui o objeto fido2AuthenticationMethod de um usuário.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador do método de autenticação.|
|displayName|Cadeia de caracteres|O nome de exibição da chave conforme dado pelo usuário.|
|createdDateTime|DateTimeOffset|O timestamp quando essa chave foi registrada para o usuário.|
|aaGuid|Cadeia de caracteres|GUID de Atestado de Autenticador, um identificador que indica o tipo (por exemplo, make e model) do autenticador.|
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

