---
title: Adicionar educationUser a uma educationSchool
description: Adicione um usuário a uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 19b61691ca020a1f5fdf8ba9dbe820b9c0d4d322
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441426"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="9ec09-103">Adicionar educationUser a uma educationSchool</span><span class="sxs-lookup"><span data-stu-id="9ec09-103">Add educationUser to an educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ec09-104">Adicione um usuário a uma escola.</span><span class="sxs-lookup"><span data-stu-id="9ec09-104">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ec09-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ec09-105">Permissions</span></span>

<span data-ttu-id="9ec09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ec09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ec09-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ec09-108">Permission type</span></span>                        | <span data-ttu-id="9ec09-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ec09-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="9ec09-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ec09-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ec09-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ec09-111">Not supported.</span></span>                              |
| <span data-ttu-id="9ec09-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ec09-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ec09-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ec09-113">Not supported.</span></span>                              |
| <span data-ttu-id="9ec09-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ec09-114">Application</span></span>                            | <span data-ttu-id="9ec09-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec09-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="9ec09-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ec09-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9ec09-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ec09-117">Request headers</span></span>

| <span data-ttu-id="9ec09-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ec09-118">Header</span></span>        | <span data-ttu-id="9ec09-119">Valor</span><span class="sxs-lookup"><span data-stu-id="9ec09-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="9ec09-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ec09-120">Authorization</span></span> | <span data-ttu-id="9ec09-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ec09-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9ec09-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ec09-123">Content-Type</span></span>  | <span data-ttu-id="9ec09-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9ec09-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="9ec09-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ec09-125">Request body</span></span>

<span data-ttu-id="9ec09-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="9ec09-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9ec09-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ec09-127">Response</span></span>

<span data-ttu-id="9ec09-128">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ec09-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ec09-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ec09-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9ec09-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ec09-130">Request</span></span>

<span data-ttu-id="9ec09-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ec09-131">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9ec09-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ec09-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->

```http
POST https://graph.microsoft.com/beta/education/schools/{id}/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14008"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ec09-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="9ec09-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ec09-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9ec09-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9ec09-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ec09-135">Response</span></span>

<span data-ttu-id="9ec09-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ec09-136">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
