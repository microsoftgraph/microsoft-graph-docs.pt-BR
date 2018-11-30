---
title: Excluir educationSchool
description: Exclua uma escola.
ms.openlocfilehash: 6ae69b725021c2a3e0a2776e8593c4346c5c6e34
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036610"
---
# <a name="delete-educationschool"></a><span data-ttu-id="de644-103">Excluir educationSchool</span><span class="sxs-lookup"><span data-stu-id="de644-103">Delete educationSchool</span></span>

> <span data-ttu-id="de644-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="de644-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de644-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="de644-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de644-106">Exclua uma escola.</span><span class="sxs-lookup"><span data-stu-id="de644-106">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="de644-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="de644-107">Permissions</span></span>
<span data-ttu-id="de644-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de644-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de644-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de644-110">Permission type</span></span>      | <span data-ttu-id="de644-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de644-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de644-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de644-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="de644-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de644-113">Not supported.</span></span>  |
|<span data-ttu-id="de644-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de644-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="de644-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de644-115">Not supported.</span></span>  |
|<span data-ttu-id="de644-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de644-116">Application</span></span> | <span data-ttu-id="de644-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de644-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="de644-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de644-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="de644-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de644-119">Request headers</span></span>
| <span data-ttu-id="de644-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de644-120">Header</span></span>       | <span data-ttu-id="de644-121">Valor</span><span class="sxs-lookup"><span data-stu-id="de644-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de644-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="de644-122">Authorization</span></span>  | <span data-ttu-id="de644-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de644-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de644-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de644-125">Request body</span></span>
<span data-ttu-id="de644-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de644-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="de644-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="de644-127">Response</span></span>
<span data-ttu-id="de644-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de644-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de644-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de644-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de644-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de644-131">Request</span></span>
<span data-ttu-id="de644-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="de644-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
##### <a name="response"></a><span data-ttu-id="de644-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="de644-133">Response</span></span>
<span data-ttu-id="de644-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="de644-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->