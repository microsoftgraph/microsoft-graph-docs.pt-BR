---
title: Excluir meetingRegistrant
description: Cancele um registro onlineMeeting para um meetingRegistrant.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8281473a3b47cede52459e8c541359af04e48972
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022003"
---
# <a name="unenroll-meeting-registrant"></a>Desemroll meeting registrant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Cancele [um registro onlineMeeting](../resources/onlinemeeting.md) para [um meetingRegistrant](../resources/meetingregistrant.md) em nome do registrante.

Use esse método somente quando a **propriedade allowedRegistrant** do [objeto meetingRegistration](../resources/meetingregistration.md) tiver um valor e a permissão delegada do registro tiver sido usada `organization` para registrar. Quando o **valor allowedRegistrant** for , os registrantes só poderão usar o link no email recebido `everyone` para cancelar o registro.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetings.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | OnlineMeetings.Read.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{userId}/onlineMeetings/{meetingId}/registration/registrants/{id}
```

>**Observações:**
>
> - `userId` é o objectID do organizador da reunião.
> - `meetingId`é a **id** de um [objeto onlineMeeting.](../resources/onlineMeeting.md)

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará apenas um `204 No Content` código de resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-registratrant-user"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/16664f75-11dc-4870-bec6-38c1aaa81431/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants/gWWckDBR6UOI8_yzWCzeNw,6pAAiSU1bkGqc8soJZw5Pg,3aMJxgQBxEufdo7_Qube_w,YgKy1Rtx-0SFjRbv-ww1ag,Cuzk8JP_iTTWqCOyVcalVA
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-registratrant-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-registratrant-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-registratrant-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-registratrant-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-registratrant-user-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "name": "delete-registratrant-user",
}-->

```http
HTTP/1.1 204 No Content
```
