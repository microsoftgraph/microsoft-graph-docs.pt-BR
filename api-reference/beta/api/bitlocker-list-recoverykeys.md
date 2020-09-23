---
title: Listar recoveryKeys
description: Obtenha uma lista dos objetos bitlockerRecoveryKey e suas propriedades.
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 566a0c81a648207d8fb719f044a6095e2ae4847e
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222875"
---
# <a name="list-recoverykeys"></a>Listar recoveryKeys
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista dos objetos [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) e suas propriedades. 

Essa operação não retorna a propriedade **Key** . Para obter informações sobre como ler a propriedade **Key** , consulte [Get bitlockerRecoveryKey](bitlockerrecoverykey-get.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|BitLocker. ReadBasic. All, BitLocker. Read. All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|Sem suporte|

>**Observação**: para permissões delegadas para permitir que os aplicativos obtenham recursos do BitLockerRecoveryKey em nome do usuário conectado, o administrador do locatário deve ter atribuído ao usuário uma das seguintes funções ou o usuário deve ser o proprietário registrado do dispositivo para o qual a chave de recuperação do BitLocker foi originalmente com backup: 
* Administrador global
* Administrador do dispositivo de nuvem
* Administrador da assistência técnica
* Administrador de Serviço do Intune
* Administrador de segurança
* Leitor de segurança
* Leitor global

## <a name="http-request"></a>Solicitação HTTP
Para obter uma lista de chaves do BitLocker dentro do locatário:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys
```

Para obter uma lista de chaves do BitLocker dentro do locatário filtrado pela **ID do dispositivo**:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys?$filter=deviceId eq '{deviceId}'
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte ao `$filter` parâmetro de consulta OData para filtrar os resultados pela **ID do dispositivo** em que o backup foi feito mais recentemente. Para obter detalhes, consulte o [exemplo 2](#example-2). Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

A resposta também pode conter um `odata.nextLink` , que você pode usar para percorrer o conjunto de resultados. Para obter detalhes, consulte [paginação de dados do Microsoft Graph](/graph/paging).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|OCP-Client-Name|Nome do aplicativo cliente executando a chamada à API. Obrigatório.|
|OCP-Client-Version|Versão do aplicativo cliente executando a chamada à API. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1"></a>Exemplo 1
Recupere uma lista de chaves do BitLocker no locatário.

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.bitlockerRecoveryKey)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "2ef04ef1-23b0-2e00-a3a5-ab345e567ab6"
    },
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "6a30ed7b-247b-4d26-86b5-2f405e55ea42",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```
### <a name="example-2"></a>Exemplo 2
Recupere uma lista de chaves do BitLocker filtradas por **ID de dispositivo**.

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleIds": ["1ab40ab2-32a8-4b00-b6b5-ba724e407de9"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys?$filter=deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.bitlockerRecoveryKey)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```
