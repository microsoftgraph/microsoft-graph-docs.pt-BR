---
title: 'educationSubmission: retornar'
description: Esta ação faz com que o nível e os comentários associados a esse envio disponível ao aluno.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: e4e5802e819543679158a3940fcf35ca624bad71
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887728"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="95de2-103">educationSubmission: retornar</span><span class="sxs-lookup"><span data-stu-id="95de2-103">educationSubmission: return</span></span>

> <span data-ttu-id="95de2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="95de2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95de2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="95de2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95de2-106">Esta ação faz com que o nível e os comentários associados a esse envio disponível ao aluno.</span><span class="sxs-lookup"><span data-stu-id="95de2-106">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="95de2-107">Isso irá alterar o status do envio de "enviado" a "retornado" e indica que o comentário for fornecido ou classificação é feito.</span><span class="sxs-lookup"><span data-stu-id="95de2-107">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="95de2-108">Essa ação só pode ser feita com o professor.</span><span class="sxs-lookup"><span data-stu-id="95de2-108">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="95de2-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="95de2-109">Permissions</span></span>
<span data-ttu-id="95de2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95de2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95de2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95de2-112">Permission type</span></span>      | <span data-ttu-id="95de2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95de2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95de2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95de2-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="95de2-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95de2-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="95de2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95de2-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="95de2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95de2-117">Not supported.</span></span>  |
|<span data-ttu-id="95de2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95de2-118">Application</span></span> | <span data-ttu-id="95de2-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95de2-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="95de2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95de2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="95de2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95de2-121">Request headers</span></span>
| <span data-ttu-id="95de2-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95de2-122">Header</span></span>       | <span data-ttu-id="95de2-123">Valor</span><span class="sxs-lookup"><span data-stu-id="95de2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95de2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="95de2-124">Authorization</span></span>  | <span data-ttu-id="95de2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95de2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95de2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95de2-127">Request body</span></span>
<span data-ttu-id="95de2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95de2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95de2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="95de2-129">Response</span></span>
<span data-ttu-id="95de2-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95de2-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95de2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95de2-132">Example</span></span>
<span data-ttu-id="95de2-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="95de2-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="95de2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95de2-134">Request</span></span>
<span data-ttu-id="95de2-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="95de2-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="95de2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="95de2-136">Response</span></span>
<span data-ttu-id="95de2-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="95de2-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
