---
title: Excluir onlineMeeting
description: Excluir uma reunião online.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: fb05bb2746a68d307a46651498163e570c7ca0f2
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516154"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="cc965-103">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="cc965-103">Delete onlineMeeting</span></span>

<span data-ttu-id="cc965-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc965-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc965-105">Excluir um [objeto onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="cc965-105">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc965-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc965-106">Permissions</span></span>

| <span data-ttu-id="cc965-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc965-107">Permission type</span></span> | <span data-ttu-id="cc965-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc965-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="cc965-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc965-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc965-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc965-110">OnlineMeetings.ReadWrite</span></span>              |
| <span data-ttu-id="cc965-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc965-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc965-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc965-112">Not Supported.</span></span>                         |
| <span data-ttu-id="cc965-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc965-113">Application</span></span>                            | <span data-ttu-id="cc965-114">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="cc965-114">OnlineMeetings.ReadWrite.All\*</span></span>          |

> [!IMPORTANT]
> <span data-ttu-id="cc965-115">\*Os administradores [](/graph/cloud-communication-online-meeting-application-access-policy) devem criar uma política de acesso a aplicativos e concedi-la a um usuário, autorizando o aplicativo configurado na política para excluir uma reunião online em nome desse usuário (ID do usuário especificada no caminho de reuqest) foi criada.</span><span class="sxs-lookup"><span data-stu-id="cc965-115">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to delete an online meeting on behalf of that user (user ID specified in the reuqest path) has created.</span></span>

## <a name="http-request"></a><span data-ttu-id="cc965-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc965-116">HTTP request</span></span>
<span data-ttu-id="cc965-117">Para excluir o onlineMeeting especificado por ID de reunião com permissão delegada:</span><span class="sxs-lookup"><span data-stu-id="cc965-117">To delete the specified onlineMeeting by meeting ID with delegated permission:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="cc965-118">Para excluir o onlineMeeting especificado por meio da ID de reunião com a permissão do aplicativo:</span><span class="sxs-lookup"><span data-stu-id="cc965-118">To delete the specified onlineMeeting by meeting ID with application permission:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{userId}/onlineMeetings/{meetingId}
```
> <span data-ttu-id="cc965-119">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="cc965-119">**Note:**</span></span>
> - <span data-ttu-id="cc965-120">`userId`é a ID do objeto de um usuário no portal de gerenciamento [de usuários do Azure.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="cc965-120">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="cc965-121">Para obter mais detalhes, consulte [política de acesso ao aplicativo](/graph/cloud-communication-online-meeting-application-access-policy).</span><span class="sxs-lookup"><span data-stu-id="cc965-121">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="cc965-122">`meetingId`é a **id** de um [objeto onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="cc965-122">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc965-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc965-123">Request headers</span></span>
| <span data-ttu-id="cc965-124">Nome</span><span class="sxs-lookup"><span data-stu-id="cc965-124">Name</span></span>          | <span data-ttu-id="cc965-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc965-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cc965-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc965-126">Authorization</span></span> | <span data-ttu-id="cc965-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc965-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc965-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc965-129">Request body</span></span>
<span data-ttu-id="cc965-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc965-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc965-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc965-131">Response</span></span>
<span data-ttu-id="cc965-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc965-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc965-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cc965-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cc965-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc965-135">Request</span></span>
<span data-ttu-id="cc965-136">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc965-136">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc965-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc965-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype"],
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="c"></a>[<span data-ttu-id="cc965-138">C#</span><span class="sxs-lookup"><span data-stu-id="cc965-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc965-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc965-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc965-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc965-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc965-141">Java</span><span class="sxs-lookup"><span data-stu-id="cc965-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cc965-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc965-142">Response</span></span>

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

