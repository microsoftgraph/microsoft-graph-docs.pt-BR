---
title: Excluir categoria do Outlook
description: Exclua o objeto outlookCategory especificado.
ms.openlocfilehash: 4e28eff91c582fcb234c69cb9930c64c84d71724
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006829"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="4180a-103">Excluir categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="4180a-103">Delete Outlook category</span></span>


<span data-ttu-id="4180a-104">Exclua o objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="4180a-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4180a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4180a-105">Permissions</span></span>
<span data-ttu-id="4180a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4180a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4180a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4180a-108">Permission type</span></span>      | <span data-ttu-id="4180a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4180a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4180a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4180a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4180a-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4180a-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="4180a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4180a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4180a-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4180a-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="4180a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4180a-114">Application</span></span> | <span data-ttu-id="4180a-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4180a-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4180a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4180a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4180a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4180a-117">Optional query parameters</span></span>
<span data-ttu-id="4180a-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4180a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4180a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4180a-119">Request headers</span></span>
| <span data-ttu-id="4180a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4180a-120">Name</span></span>      |<span data-ttu-id="4180a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4180a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4180a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4180a-122">Authorization</span></span>  | <span data-ttu-id="4180a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4180a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4180a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4180a-125">Request body</span></span>
<span data-ttu-id="4180a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4180a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4180a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4180a-127">Response</span></span>

<span data-ttu-id="4180a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4180a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4180a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4180a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4180a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4180a-131">Request</span></span>
<span data-ttu-id="4180a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4180a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="4180a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4180a-133">Response</span></span>
<span data-ttu-id="4180a-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4180a-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->