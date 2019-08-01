---
title: Criar categoria do Outlook
description: Cria um objeto outlookCategory na lista mestra de categorias do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: be7ec5bc9437cb9fc13c3f89c10747f5ea75e2da
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976310"
---
# <a name="create-outlook-category"></a><span data-ttu-id="2461c-103">Criar categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="2461c-103">Create Outlook category</span></span>


<span data-ttu-id="2461c-104">Cria um objeto [outlookCategory](../resources/outlookcategory.md) na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="2461c-104">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="2461c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2461c-105">Permissions</span></span>
<span data-ttu-id="2461c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2461c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2461c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2461c-108">Permission type</span></span>      | <span data-ttu-id="2461c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2461c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2461c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2461c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2461c-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2461c-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="2461c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2461c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2461c-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2461c-113">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="2461c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2461c-114">Application</span></span> | <span data-ttu-id="2461c-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2461c-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2461c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2461c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="2461c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2461c-117">Request headers</span></span>
| <span data-ttu-id="2461c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2461c-118">Name</span></span>       | <span data-ttu-id="2461c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2461c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2461c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2461c-120">Authorization</span></span>  | <span data-ttu-id="2461c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2461c-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2461c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2461c-123">Request body</span></span>
<span data-ttu-id="2461c-124">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="2461c-124">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2461c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2461c-125">Response</span></span>

<span data-ttu-id="2461c-126">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2461c-126">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2461c-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2461c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2461c-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2461c-128">Request</span></span>
<span data-ttu-id="2461c-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2461c-129">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2461c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2461c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2461c-131">C#</span><span class="sxs-lookup"><span data-stu-id="2461c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlookcategory-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2461c-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="2461c-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlookcategory-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2461c-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2461c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlookcategory-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2461c-134">Java</span><span class="sxs-lookup"><span data-stu-id="2461c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlookcategory-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2461c-135">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="2461c-135">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2461c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2461c-136">Response</span></span>
<span data-ttu-id="2461c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2461c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
