---
title: Obter contactMergeSuggestions
description: Leia as propriedades e as relações de um objeto contactMergeSuggestions.
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 108e6b724885507d8d51e0b5049b1dc4e68d98c1
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338038"
---
# <a name="get-contactmergesuggestions"></a>Obter contactMergeSuggestions
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto contactMergeSuggestions](../resources/contactmergesuggestions.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|User.Read, User.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/settings/contactMergeSuggestions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um [objeto contactMergeSuggestions](../resources/contactmergesuggestions.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

A seguir, um exemplo da solicitação para obter as **configurações contactMergeSuggestions** para o usuário.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_contactmergesuggestions"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/settings/contactMergeSuggestions
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactMergeSuggestions",
  "name": "get_contactmergesuggestions"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "isEnabled": true
}
```

