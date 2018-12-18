---
title: 'educationSubmission: retornar'
description: Esta ação faz com que o nível e os comentários associados a esse envio disponível ao aluno.
author: dipakboyed
ms.openlocfilehash: d73300328168baf9481b329b36f056aa27044b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350873"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="8428c-103">educationSubmission: retornar</span><span class="sxs-lookup"><span data-stu-id="8428c-103">educationSubmission: return</span></span>

> <span data-ttu-id="8428c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8428c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8428c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8428c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8428c-106">Esta ação faz com que o nível e os comentários associados a esse envio disponível ao aluno.</span><span class="sxs-lookup"><span data-stu-id="8428c-106">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="8428c-107">Isso irá alterar o status do envio de "enviado" a "retornado" e indica que o comentário for fornecido ou classificação é feito.</span><span class="sxs-lookup"><span data-stu-id="8428c-107">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="8428c-108">Essa ação só pode ser feita com o professor.</span><span class="sxs-lookup"><span data-stu-id="8428c-108">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="8428c-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8428c-109">Permissions</span></span>
<span data-ttu-id="8428c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8428c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8428c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8428c-112">Permission type</span></span>      | <span data-ttu-id="8428c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8428c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8428c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8428c-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="8428c-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8428c-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="8428c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8428c-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8428c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8428c-117">Not supported.</span></span>  |
|<span data-ttu-id="8428c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8428c-118">Application</span></span> | <span data-ttu-id="8428c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8428c-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8428c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8428c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="8428c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8428c-121">Request headers</span></span>
| <span data-ttu-id="8428c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8428c-122">Header</span></span>       | <span data-ttu-id="8428c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8428c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8428c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8428c-124">Authorization</span></span>  | <span data-ttu-id="8428c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8428c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8428c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8428c-127">Request body</span></span>
<span data-ttu-id="8428c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8428c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8428c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8428c-129">Response</span></span>
<span data-ttu-id="8428c-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8428c-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8428c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8428c-132">Example</span></span>
<span data-ttu-id="8428c-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8428c-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8428c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8428c-134">Request</span></span>
<span data-ttu-id="8428c-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8428c-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="8428c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8428c-136">Response</span></span>
<span data-ttu-id="8428c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8428c-137">The following is an example of the response.</span></span>

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