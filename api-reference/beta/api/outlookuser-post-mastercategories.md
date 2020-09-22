---
title: Criar categoria do Outlook
description: Cria um objeto outlookCategory na lista mestra de categorias do usuário.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 35c40867797a6b65e4f45a1de2f4b2a854a50b72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053395"
---
# <a name="create-outlook-category"></a><span data-ttu-id="1ac68-103">Criar categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="1ac68-103">Create Outlook category</span></span>

<span data-ttu-id="1ac68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ac68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ac68-105">Cria um objeto [outlookCategory](../resources/outlookcategory.md) na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="1ac68-105">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ac68-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ac68-106">Permissions</span></span>
<span data-ttu-id="1ac68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ac68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ac68-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ac68-109">Permission type</span></span>      | <span data-ttu-id="1ac68-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ac68-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ac68-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ac68-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1ac68-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ac68-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1ac68-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ac68-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ac68-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ac68-114">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="1ac68-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ac68-115">Application</span></span> | <span data-ttu-id="1ac68-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ac68-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ac68-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ac68-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="1ac68-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ac68-118">Request headers</span></span>
| <span data-ttu-id="1ac68-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1ac68-119">Name</span></span>       | <span data-ttu-id="1ac68-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ac68-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1ac68-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ac68-121">Authorization</span></span>  | <span data-ttu-id="1ac68-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ac68-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1ac68-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ac68-124">Request body</span></span>
<span data-ttu-id="1ac68-125">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="1ac68-125">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1ac68-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ac68-126">Response</span></span>

<span data-ttu-id="1ac68-127">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ac68-127">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ac68-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ac68-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ac68-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ac68-129">Request</span></span>
<span data-ttu-id="1ac68-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ac68-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ac68-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ac68-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1ac68-132">C#</span><span class="sxs-lookup"><span data-stu-id="1ac68-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlookcategory-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ac68-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ac68-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlookcategory-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ac68-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ac68-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlookcategory-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1ac68-135">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="1ac68-135">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1ac68-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ac68-136">Response</span></span>
<span data-ttu-id="1ac68-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ac68-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


