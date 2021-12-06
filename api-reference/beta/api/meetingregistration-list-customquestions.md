---
title: Listar customQuestions
description: Obter uma lista das perguntas de registro personalizadas associadas a um objeto meetingRegistration.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: da15e5fce703276103ed70dea4a96465b672c97c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011790"
---
# <a name="list-customquestions"></a>Listar customQuestions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista das perguntas [de registro personalizadas](../resources/meetingregistrationquestion.md) associadas a um [objeto meetingRegistration](../resources/meetingregistration.md) em nome do organizador.

> [!TIP]
> Você também pode usar a [operação Obter meetingRegistration](meetingregistration-get.md) para obter perguntas de registro personalizadas.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetings.Read, OnlineMeetings.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{id}/registration/customQuestions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos meetingRegistrationQuestion](../resources/meetingregistrationquestion.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list-custom-questions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/customQuestions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-custom-questions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-custom-questions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-custom-questions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-custom-questions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-custom-questions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

> **Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.

<!-- {
  "blockType": "response",
  "name": "list-custom-questions",
  "@odata.type": "Collection(microsoft.graph.meetingRegistrationQuestion)"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/customQuestions",
  "value": [
    {
      "id": "MSMxY2E2ZmE3OS1hOTY3LTQ4ZX3lvdV94MDAyMF9hX3gwMDIwX2RldmU=",
      "displayName": "Are you a developer?",
      "isRequired": true,
      "answerInputType": "radioButton",
      "answerOptions": [
        "Yes",
        "No"
      ]
    },
    {
      "id": "MSM4YzZhMTkTQjV2hlcmVfeDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=",
      "displayName": "Where did you hear about us?",
      "isRequired": false,
      "answerInputType": "text",
      "answerOptions": []
    }
  ]
}
```
