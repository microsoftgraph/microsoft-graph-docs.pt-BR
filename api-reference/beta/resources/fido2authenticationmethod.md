---
title: tipo de recurso fido2AuthenticationMethod
description: Uma representação de uma chave de segurança do FIDO2 registrada para um usuário. FIDO2 é um método de autenticação de entrada.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c4d10252201781d1339e6baa26aea248429ae462
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418173"
---
# <a name="fido2authenticationmethod-resource-type"></a>tipo de recurso fido2AuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação de uma chave de segurança do FIDO2 registrada para um usuário. FIDO2 é um método de autenticação de entrada.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List](../api/fido2authenticationmethod-list.md)|coleção [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Recupere uma lista de objetos fido2AuthenticationMethod de um usuário e suas propriedades.|
|[Obter](../api/fido2authenticationmethod-get.md)|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Leia as propriedades e os relacionamentos do objeto fido2AuthenticationMethod de um usuário.|
|[Excluir](../api/fido2authenticationmethod-delete.md)|Nenhum|Exclui o objeto fido2AuthenticationMethod de um usuário.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador do método de autenticação.|
|displayName|Cadeia de caracteres|O nome de exibição da chave, conforme fornecido pelo usuário.|
|creationDatetime|DateTimeOffset|O carimbo de data/hora em que essa chave foi registrada para o usuário.|
|aaGuid|Cadeia de caracteres|GUID de atestado de autenticador, um identificador que indica o tipo (por exemplo, Make e Model) do autenticador.|
|modelo|String|O modelo atribuído pelo fabricante da chave de segurança FIDO2.|
|attestationCertificates|Conjunto de cadeias de caracteres|Os certificados de atestado anexados a essa chave de segurança.|
|attestationLevel|attestationLevel|O nível de atestado dessa chave de segurança do FIDO2. Os valores possíveis são: `attested` , ou `notAttested` .|


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

