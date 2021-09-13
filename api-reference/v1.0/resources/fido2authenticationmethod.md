---
title: Tipo de recurso fido2AuthenticationMethod
description: Uma representação de uma chave de segurança FIDO2 registrada em um usuário. FIDO2 é um método de autenticação de login.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8af931dba72daba05c8c548cc53d130d6f3f182b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062716"
---
# <a name="fido2authenticationmethod-resource-type"></a>Tipo de recurso fido2AuthenticationMethod

Namespace: microsoft.graph

Uma representação de uma chave de segurança FIDO2 registrada em um usuário. FIDO2 é um método de autenticação de login.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List](../api/fido2authenticationmethod-list.md)|[coleção fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Recupere uma lista dos objetos fido2AuthenticationMethod de um usuário e suas propriedades.|
|[Obter](../api/fido2authenticationmethod-get.md)|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Leia as propriedades e as relações do objeto fido2AuthenticationMethod de um usuário.|
|[Delete](../api/fido2authenticationmethod-delete.md)|None|Exclui o objeto fido2AuthenticationMethod de um usuário.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do método de autenticação.|
|displayName|Cadeia de caracteres|O nome de exibição da chave conforme dado pelo usuário.|
|createdDateTime|DateTimeOffset|O timestamp quando essa chave foi registrada para o usuário.|
|aaGuid|Cadeia de caracteres|Authenticator GUID de atestado, um identificador que indica o tipo (por exemplo, make e model) do autenticador.|
|modelo|String|O modelo atribuído pelo fabricante da chave de segurança FIDO2.|
|attestationCertificates|Coleção String|Os certificados de atestado anexados a essa chave de segurança.|
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
  "createdDateTime": "String (timestamp)",
  "aaGuid": "String",
  "model": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String"
}
```

