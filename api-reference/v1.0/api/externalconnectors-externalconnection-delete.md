---
title: Excluir externalConnection
description: Exclui um objeto externalConnection.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 1a34627d95b2e65798c93fae1bf45beb3772b93f
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560008"
---
# <a name="delete-externalconnection"></a>Excluir externalConnection
Namespace: microsoft.graph.externalConnectors



Exclui um [objeto externalConnection.](../resources/externalconnectors-externalconnection.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Não aplicável|
|Delegado (conta pessoal da Microsoft)|Não aplicável|
|Application| ExternalConnection.ReadWrite.OwnedBy|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /external/connections/{connectionsId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "delete_externalconnection"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/external/connections/contosohr
```



### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

