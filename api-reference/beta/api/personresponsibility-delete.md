---
title: Excluir personResponsibility
description: Exclui um objeto personResponsibility.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8e5ae2fecc8c1845712b1d15161694da9c215ae1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986235"
---
# <a name="delete-personresponsibility"></a>Excluir personResponsibility
Namespace: microsoft.graph

Exclui um objeto [personResponsibility](../resources/personresponsibility.md) do [perfil](../resources/profile.md)de um usuário.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All |
| Delegado (conta pessoal da Microsoft) | User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All |
| Aplicativo                            | User. ReadBasic. All, User. Read. All, User. ReadWrite. All                            |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/responsibilities/{id}
DELETE /users/{id | userPrincipalName}/profile/responsibilities/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "delete_personresponsibility"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/profile/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


