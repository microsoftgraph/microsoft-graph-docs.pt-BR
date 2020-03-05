---
title: Criar categoria do Outlook
description: Cria um objeto outlookCategory na lista mestra de categorias do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 55a60cf5ab8d7be5df4a8d0c29fe646131bf1651
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456072"
---
# <a name="create-outlook-category"></a><span data-ttu-id="c6a60-103">Criar categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="c6a60-103">Create Outlook category</span></span>

<span data-ttu-id="c6a60-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c6a60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6a60-105">Cria um objeto [outlookCategory](../resources/outlookcategory.md) na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6a60-105">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6a60-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6a60-106">Permissions</span></span>
<span data-ttu-id="c6a60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6a60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6a60-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6a60-109">Permission type</span></span>      | <span data-ttu-id="c6a60-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6a60-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6a60-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6a60-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c6a60-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6a60-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c6a60-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6a60-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6a60-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6a60-114">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="c6a60-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6a60-115">Application</span></span> | <span data-ttu-id="c6a60-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6a60-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6a60-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6a60-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="c6a60-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6a60-118">Request headers</span></span>
| <span data-ttu-id="c6a60-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c6a60-119">Name</span></span>       | <span data-ttu-id="c6a60-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6a60-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c6a60-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6a60-121">Authorization</span></span>  | <span data-ttu-id="c6a60-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6a60-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c6a60-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6a60-124">Request body</span></span>
<span data-ttu-id="c6a60-125">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="c6a60-125">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c6a60-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6a60-126">Response</span></span>

<span data-ttu-id="c6a60-127">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6a60-127">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6a60-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6a60-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6a60-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6a60-129">Request</span></span>
<span data-ttu-id="c6a60-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6a60-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c6a60-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6a60-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
# <a name="c"></a>[<span data-ttu-id="c6a60-132">C#</span><span class="sxs-lookup"><span data-stu-id="c6a60-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlookcategory-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6a60-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6a60-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlookcategory-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6a60-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6a60-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlookcategory-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c6a60-135">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="c6a60-135">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c6a60-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6a60-136">Response</span></span>
<span data-ttu-id="c6a60-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6a60-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
