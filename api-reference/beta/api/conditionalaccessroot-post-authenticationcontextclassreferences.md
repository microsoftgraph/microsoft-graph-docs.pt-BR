---
title: Criar authenticationContextClassReference
description: Crie uma nova autenticaçãoContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4646e8a388800587c0aa73a736d591dc6b97c6fb
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663933"
---
# <a name="create-authenticationcontextclassreference"></a><span data-ttu-id="31412-103">Criar authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="31412-103">Create authenticationContextClassReference</span></span>

<span data-ttu-id="31412-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31412-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31412-105">Criar uma nova [autenticaçãoContextClassReference](../resources/authenticationContextClassReference.md).</span><span class="sxs-lookup"><span data-stu-id="31412-105">Create a new [authenticationContextClassReference](../resources/authenticationContextClassReference.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="31412-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="31412-106">Permissions</span></span>

<span data-ttu-id="31412-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31412-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31412-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31412-109">Permission type</span></span>                        | <span data-ttu-id="31412-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31412-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="31412-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31412-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="31412-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="31412-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="31412-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31412-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31412-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31412-114">Not supported.</span></span> |
|<span data-ttu-id="31412-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31412-115">Application</span></span>                            | <span data-ttu-id="31412-116">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="31412-116">Policy.ReadWrite.ConditionalAccess</span></span> |

> [!NOTE]
> <span data-ttu-id="31412-117">Essa API tem um [problema conhecido relacionado](/graph/known-issues#permissions) a permissões.</span><span class="sxs-lookup"><span data-stu-id="31412-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="31412-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31412-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/authenticationContextClassReferences
```

## <a name="request-headers"></a><span data-ttu-id="31412-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31412-119">Request headers</span></span>

| <span data-ttu-id="31412-120">Nome</span><span class="sxs-lookup"><span data-stu-id="31412-120">Name</span></span>          | <span data-ttu-id="31412-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="31412-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="31412-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="31412-122">Authorization</span></span> | <span data-ttu-id="31412-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31412-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="31412-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31412-125">Content-Type</span></span>  | <span data-ttu-id="31412-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31412-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31412-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31412-128">Request body</span></span>

<span data-ttu-id="31412-129">No corpo da solicitação, fornece uma representação JSON de um [objeto authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="31412-129">In the request body, supply a JSON representation of a [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="31412-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="31412-130">Response</span></span>

<span data-ttu-id="31412-131">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto authenticationContextClassReference](../resources/authenticationcontextclassreference.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31412-131">If successful, this method returns a `201 Created` response code and a new [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31412-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="31412-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31412-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31412-133">Request</span></span>
<span data-ttu-id="31412-134">O exemplo a seguir mostra a criação de uma nova authenticationcontextclassreference que está disponível para aplicativos usarem.</span><span class="sxs-lookup"><span data-stu-id="31412-134">The following example shows creating a new authenticationcontextclassreference that is available for apps to use.</span></span>




# <a name="http"></a>[<span data-ttu-id="31412-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="31412-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_authenticationcontextclassreference"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences
Content-type: application/json

{
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```
# <a name="c"></a>[<span data-ttu-id="31412-136">C#</span><span class="sxs-lookup"><span data-stu-id="31412-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-authenticationcontextclassreference-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31412-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31412-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-authenticationcontextclassreference-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31412-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31412-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-authenticationcontextclassreference-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31412-139">Java</span><span class="sxs-lookup"><span data-stu-id="31412-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-authenticationcontextclassreference-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a><span data-ttu-id="31412-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="31412-140">Response</span></span>

<span data-ttu-id="31412-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31412-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.authenticationContextClassReference"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/authenticationContextClassReference/$entity",
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
