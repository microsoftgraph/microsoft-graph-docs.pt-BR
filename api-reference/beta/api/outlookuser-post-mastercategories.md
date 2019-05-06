---
title: Criar categoria do Outlook
description: Cria um objeto outlookCategory na lista mestra de categorias do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4b80a7794430bcfb82f11f515959a96027458d0a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596057"
---
# <a name="create-outlook-category"></a><span data-ttu-id="99141-103">Criar categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="99141-103">Create Outlook category</span></span>


<span data-ttu-id="99141-104">Cria um objeto [outlookCategory](../resources/outlookcategory.md) na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="99141-104">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="99141-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="99141-105">Permissions</span></span>
<span data-ttu-id="99141-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99141-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99141-108">Permission type</span></span>      | <span data-ttu-id="99141-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99141-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99141-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99141-110">Delegated (work or school account)</span></span> | <span data-ttu-id="99141-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99141-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="99141-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99141-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99141-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99141-113">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="99141-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99141-114">Application</span></span> | <span data-ttu-id="99141-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99141-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="99141-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99141-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="99141-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99141-117">Request headers</span></span>
| <span data-ttu-id="99141-118">Nome</span><span class="sxs-lookup"><span data-stu-id="99141-118">Name</span></span>       | <span data-ttu-id="99141-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="99141-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="99141-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="99141-120">Authorization</span></span>  | <span data-ttu-id="99141-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99141-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="99141-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99141-123">Request body</span></span>
<span data-ttu-id="99141-124">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="99141-124">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="99141-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="99141-125">Response</span></span>

<span data-ttu-id="99141-126">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99141-126">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99141-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99141-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99141-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99141-128">Request</span></span>
<span data-ttu-id="99141-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99141-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="99141-130">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="99141-130">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="99141-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="99141-131">Response</span></span>
<span data-ttu-id="99141-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99141-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="99141-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="99141-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="99141-136">Basic</span><span class="sxs-lookup"><span data-stu-id="99141-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_outlookcategory_from_outlookuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99141-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99141-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_outlookcategory_from_outlookuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/outlookuser-post-mastercategories.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookuser-post-mastercategories.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
