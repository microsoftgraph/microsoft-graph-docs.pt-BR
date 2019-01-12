---
title: Excluir educationSchool
description: Exclua uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4fb4735a60303e252d75a8a4cebb39d2f4c252a4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950582"
---
# <a name="delete-educationschool"></a><span data-ttu-id="0e157-103">Excluir educationSchool</span><span class="sxs-lookup"><span data-stu-id="0e157-103">Delete educationSchool</span></span>

> <span data-ttu-id="0e157-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0e157-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e157-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0e157-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e157-106">Exclua uma escola.</span><span class="sxs-lookup"><span data-stu-id="0e157-106">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e157-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e157-107">Permissions</span></span>
<span data-ttu-id="0e157-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e157-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e157-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e157-110">Permission type</span></span>      | <span data-ttu-id="0e157-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e157-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e157-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e157-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="0e157-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e157-113">Not supported.</span></span>  |
|<span data-ttu-id="0e157-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e157-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0e157-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e157-115">Not supported.</span></span>  |
|<span data-ttu-id="0e157-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e157-116">Application</span></span> | <span data-ttu-id="0e157-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e157-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0e157-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e157-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0e157-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e157-119">Request headers</span></span>
| <span data-ttu-id="0e157-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e157-120">Header</span></span>       | <span data-ttu-id="0e157-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0e157-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0e157-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e157-122">Authorization</span></span>  | <span data-ttu-id="0e157-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e157-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e157-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e157-125">Request body</span></span>
<span data-ttu-id="0e157-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e157-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0e157-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e157-127">Response</span></span>
<span data-ttu-id="0e157-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e157-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e157-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e157-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e157-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e157-131">Request</span></span>
<span data-ttu-id="0e157-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e157-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
##### <a name="response"></a><span data-ttu-id="0e157-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e157-133">Response</span></span>
<span data-ttu-id="0e157-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0e157-134">The following is an example of the response.</span></span> 

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
