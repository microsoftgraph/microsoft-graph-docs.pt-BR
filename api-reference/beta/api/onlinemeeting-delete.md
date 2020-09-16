---
title: Excluir onlineMeeting
description: Excluir uma reunião online.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 051db73f098272bc97fe3477e6bd8dd3f49eddf5
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843265"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="dd834-103">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="dd834-103">Delete onlineMeeting</span></span>

<span data-ttu-id="dd834-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd834-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd834-105">Excluir um objeto [onlineMeeting](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="dd834-105">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd834-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd834-106">Permissions</span></span>

| <span data-ttu-id="dd834-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd834-107">Permission type</span></span>                        | <span data-ttu-id="dd834-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd834-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="dd834-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd834-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd834-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd834-110">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="dd834-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd834-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd834-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd834-112">Not Supported.</span></span>                              |
| <span data-ttu-id="dd834-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd834-113">Application</span></span>                            | <span data-ttu-id="dd834-114">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="dd834-114">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="dd834-115">\* Os administradores devem criar uma [política de acesso de aplicativo](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md) e conceder a ele um usuário, autorizando o aplicativo configurado na política para excluir uma reunião online em nome desse usuário (a ID de usuário especificada no caminho reuqest) foi criada.</span><span class="sxs-lookup"><span data-stu-id="dd834-115">\* Administrators must create an [application access policy](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md) and grant it to a user, authorizing the app configured in the policy to delete an online meeting on behalf of that user (user ID specified in the reuqest path) has created.</span></span>

## <a name="http-request"></a><span data-ttu-id="dd834-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd834-116">HTTP request</span></span>

<span data-ttu-id="dd834-117">Solicitação ao usar um token delegado</span><span class="sxs-lookup"><span data-stu-id="dd834-117">Request when using a delegated token</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/{meetingId}
```

<span data-ttu-id="dd834-118">Solicitação ao usar um token de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="dd834-118">Request when using an application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/users/{userId}/onlineMeetings/{meetingId}
```

> <span data-ttu-id="dd834-119">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="dd834-119">**Note:**</span></span>
>
> - <span data-ttu-id="dd834-120">`userId` é a ID de objeto de um usuário no [portal de gerenciamento do usuário do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span><span class="sxs-lookup"><span data-stu-id="dd834-120">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="dd834-121">Para mais detalhes, consulte [política de acesso de aplicativo](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md).</span><span class="sxs-lookup"><span data-stu-id="dd834-121">For more details, see [application access policy](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md).</span></span>
> - <span data-ttu-id="dd834-122">`meetingId` é a **ID** de uma [entidade onlineMeeting](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="dd834-122">`meetingId` is the **id** of an [onlineMeeting entity](../resources/onlinemeeting.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd834-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd834-123">Request headers</span></span>
| <span data-ttu-id="dd834-124">Nome</span><span class="sxs-lookup"><span data-stu-id="dd834-124">Name</span></span>          | <span data-ttu-id="dd834-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd834-125">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dd834-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd834-126">Authorization</span></span> | <span data-ttu-id="dd834-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd834-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd834-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd834-129">Request body</span></span>
<span data-ttu-id="dd834-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd834-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd834-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd834-131">Response</span></span>
<span data-ttu-id="dd834-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd834-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd834-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dd834-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dd834-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd834-135">Request</span></span>
<span data-ttu-id="dd834-136">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd834-136">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dd834-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd834-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="c"></a>[<span data-ttu-id="dd834-138">C#</span><span class="sxs-lookup"><span data-stu-id="dd834-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd834-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd834-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd834-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd834-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dd834-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd834-141">Response</span></span>

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
