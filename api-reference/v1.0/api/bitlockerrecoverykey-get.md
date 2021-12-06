---
title: Obter bitlockerRecoveryKey
description: Recupere as propriedades e as relações de um objeto bitlockerRecoveryKey.
author: hafowler
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1a7da6ef2b5bf4fbedc75410a228f54460b30d80
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001101"
---
# <a name="get-bitlockerrecoverykey"></a>Obter bitlockerRecoveryKey
Namespace: microsoft.graph

Recupere as propriedades e as relações de um [objeto bitlockerRecoveryKey.](../resources/bitlockerrecoverykey.md) 

Por padrão, essa operação não retorna a propriedade **key** que representa a chave de recuperação real. Para incluir a **propriedade key** na resposta, use o parâmetro de `$select` consulta OData. Incluir o parâmetro de consulta dispara uma auditoria do Azure AD da operação `$select` e gera um log de auditoria. Para obter mais informações sobre logs de auditoria para chaves de recuperação do bitlocker, consulte o filtro de categoria KeyManagement dos logs de auditoria [do Azure AD.](/azure/active-directory/reports-monitoring/concept-audit-logs)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|BitLockerKey.ReadBasic.All, BitLockerKey.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|Sem suporte|

Para permissões delegadas, o usuário de chamada deve ser o proprietário registrado do dispositivo do qual a chave de recuperação do BitLocker foi originalmente backup, ou ele deve estar em uma das seguintes funções de [diretório:](/azure/active-directory/roles/permissions-reference)
* Administrador global
* Administrador de dispositivos de nuvem
* Administrador da assistência técnica
* Administrador de Serviço do Intune
* Administrador de segurança
* Leitor de segurança
* Leitor global

## <a name="http-request"></a>Solicitação HTTP
Para obter a chave BitLocker especificada sem retornar a **propriedade key:**
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/{bitlockeryRecoveryKeyId}
```

Para obter a chave BitLocker especificada, incluindo sua **propriedade chave:**
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/{bitlockeryRecoveryKeyId}?$select=key
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte ao `$select` parâmetro de consulta OData para retornar a **propriedade key.** Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|ocp-client-name|O nome do aplicativo cliente que executa a chamada da API. Esse header é usado para fins de depuração. Opcional.|
|ocp-client-version|A versão do aplicativo cliente que executa a chamada da API. Esse header é usado para fins de depuração. Opcional.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-bitlocker-key-by-specifying-the-key-id"></a>Exemplo 1: Obter a chave BitLocker especificando a id da chave

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação. Este exemplo não retorna a **propriedade key.**


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4
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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-bitlockerrecoverykey-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
    "createdDateTime": "2020-06-15T13:45:30.0000000Z",
    "volumeType": "1",
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
  }
}
```

### <a name="example-2-get-the-bitlocker-key-with-the-key-property"></a>Exemplo 2: Obter a chave BitLocker com a **propriedade key**

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey_key"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4?$select=key
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-key-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-key-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-key-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-key-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-bitlockerrecoverykey-key-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
    "createdDateTime": "String (timestamp)",
    "volumeType": "1",
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
    "key": "123456-231453-873456-213546-654678-765689-123456-324565"
  }
}
```
