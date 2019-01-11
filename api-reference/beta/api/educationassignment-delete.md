---
title: Excluir educationAssignment
description: Exclua uma atribuição existente. Somente professores dentro de uma classe podem excluir atribuições.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 09365c44bef4f12ad9be24f8ed30cfb0efc5c6f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874988"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="755e9-104">Excluir educationAssignment</span><span class="sxs-lookup"><span data-stu-id="755e9-104">Delete educationAssignment</span></span>

> <span data-ttu-id="755e9-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="755e9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="755e9-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="755e9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="755e9-107">Exclua uma atribuição existente.</span><span class="sxs-lookup"><span data-stu-id="755e9-107">Delete an existing assignment.</span></span> <span data-ttu-id="755e9-108">Somente professores dentro de uma classe podem excluir atribuições.</span><span class="sxs-lookup"><span data-stu-id="755e9-108">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="755e9-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="755e9-109">Permissions</span></span>
<span data-ttu-id="755e9-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="755e9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="755e9-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="755e9-112">Permission type</span></span>      | <span data-ttu-id="755e9-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="755e9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="755e9-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="755e9-114">Delegated (work or school account)</span></span>| <span data-ttu-id="755e9-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="755e9-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="755e9-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="755e9-116">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="755e9-117">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="755e9-117">Not Supported.</span></span> |
|<span data-ttu-id="755e9-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="755e9-118">Application</span></span> | <span data-ttu-id="755e9-119">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="755e9-119">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="755e9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="755e9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignments/<id>
```
## <a name="request-headers"></a><span data-ttu-id="755e9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="755e9-121">Request headers</span></span>
| <span data-ttu-id="755e9-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="755e9-122">Header</span></span>       | <span data-ttu-id="755e9-123">Valor</span><span class="sxs-lookup"><span data-stu-id="755e9-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="755e9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="755e9-124">Authorization</span></span>  | <span data-ttu-id="755e9-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="755e9-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="755e9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="755e9-127">Request body</span></span>
<span data-ttu-id="755e9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="755e9-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="755e9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="755e9-129">Response</span></span>
<span data-ttu-id="755e9-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="755e9-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="755e9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="755e9-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="755e9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="755e9-133">Request</span></span>
<span data-ttu-id="755e9-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="755e9-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="755e9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="755e9-135">Response</span></span>
<span data-ttu-id="755e9-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="755e9-136">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
