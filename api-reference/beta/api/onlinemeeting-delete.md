---
title: Excluir onlineMeeting
description: Excluir uma reunião online.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 991e8f70e2505b230c7091695abe2c594a274fee
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896533"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="28613-103">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="28613-103">Delete onlineMeeting</span></span>

<span data-ttu-id="28613-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28613-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28613-105">Excluir um [objeto onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="28613-105">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="28613-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="28613-106">Permissions</span></span>

| <span data-ttu-id="28613-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28613-107">Permission type</span></span>                        | <span data-ttu-id="28613-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28613-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="28613-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28613-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="28613-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28613-110">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="28613-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28613-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28613-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28613-112">Not Supported.</span></span>                              |
| <span data-ttu-id="28613-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28613-113">Application</span></span>                            | <span data-ttu-id="28613-114">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="28613-114">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="28613-115">\*Os administradores [](/graph/cloud-communication-online-meeting-application-access-policy) devem criar uma política de acesso a aplicativos e concedi-la a um usuário, autorizando o aplicativo configurado na política para excluir uma reunião online em nome desse usuário (ID do usuário especificada no caminho de reuqest) foi criada.</span><span class="sxs-lookup"><span data-stu-id="28613-115">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to delete an online meeting on behalf of that user (user ID specified in the reuqest path) has created.</span></span>

## <a name="http-request"></a><span data-ttu-id="28613-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28613-116">HTTP request</span></span>

<span data-ttu-id="28613-117">Solicitar ao usar um token delegado</span><span class="sxs-lookup"><span data-stu-id="28613-117">Request when using a delegated token</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/{meetingId}
```

<span data-ttu-id="28613-118">Solicitar quando usar um token de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="28613-118">Request when using an application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/users/{userId}/onlineMeetings/{meetingId}
```

> [!NOTE]
> - <span data-ttu-id="28613-119">`userId` é a ID de objeto de um usuário no [Portal de gerenciamento de usuário do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span><span class="sxs-lookup"><span data-stu-id="28613-119">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="28613-120">Para obter mais detalhes, consulte [política de acesso ao aplicativo](/graph/cloud-communication-online-meeting-application-access-policy).</span><span class="sxs-lookup"><span data-stu-id="28613-120">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="28613-121">`meetingId`é a **id** de um [objeto onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="28613-121">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28613-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28613-122">Request headers</span></span>
| <span data-ttu-id="28613-123">Nome</span><span class="sxs-lookup"><span data-stu-id="28613-123">Name</span></span>          | <span data-ttu-id="28613-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="28613-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="28613-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="28613-125">Authorization</span></span> | <span data-ttu-id="28613-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28613-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28613-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28613-128">Request body</span></span>
<span data-ttu-id="28613-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28613-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28613-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="28613-130">Response</span></span>
<span data-ttu-id="28613-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28613-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28613-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="28613-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="28613-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28613-134">Request</span></span>
<span data-ttu-id="28613-135">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="28613-135">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="28613-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="28613-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype"],
  "name": "delete-call-2"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="c"></a>[<span data-ttu-id="28613-137">C#</span><span class="sxs-lookup"><span data-stu-id="28613-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28613-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28613-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28613-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28613-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28613-140">Java</span><span class="sxs-lookup"><span data-stu-id="28613-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="28613-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="28613-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


