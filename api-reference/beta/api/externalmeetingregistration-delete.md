---
title: Excluir externalMeetingRegistration
description: Desabilitar e excluir um registro de reunião externo.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a8b5e59faacb88efb68b54e7fea9b7dcb6fe78dd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113570"
---
# <a name="delete-externalmeetingregistration"></a>Excluir externalMeetingRegistration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Desabilitar e excluir [o externalMeetingRegistration](../resources/externalmeetingregistration.md) de um [onlineMeeting](../resources/onlinemeeting.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetings.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | OnlineMeetings.ReadWrite.All |

Para usar a permissão do aplicativo para [](/graph/cloud-communication-online-meeting-application-access-policy) essa API, os administradores de locatários devem criar uma política de acesso a aplicativos e concedi-la a um usuário para autorizar o aplicativo configurado na política a buscar reuniões online e/ou artefatos de reunião online em nome desse usuário (com a ID do usuário especificada no caminho da solicitação).

## <a name="http-request"></a>Solicitação HTTP

Para excluir o registro de reunião externa com permissão delegada ( `/me` ) e app ( ) `/users/{userId}/` :

<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onlineMeetings/{meetingId}/registration
DELETE /users/{userId}/onlineMeetings/{meetingId}/registration
```

> [!TIP]
>
>- `userId` é o **objectId** do organizador da reunião.
>- `meetingId`é a **id** do [objeto onlineMeeting.](../resources/onlinemeeting.md)

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará apenas um `204 No Content` código de resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-external-registration"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-external-registration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-external-registration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-external-registration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-external-registration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-external-registration-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-external-registration-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "name": "delete-external-registration"
}-->

```http
HTTP/1.1 204 No Content
```
