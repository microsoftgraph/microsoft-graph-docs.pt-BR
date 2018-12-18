---
title: 'educationSubmission: recall'
description: 'Indica que um estudante deseja reassumir o envio de um. Essa ação só pode ser feita por um estudante. '
author: dipakboyed
ms.openlocfilehash: ad49302ac9010923d0da2e31686ae4f6967bb50b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302314"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="e1f06-104">educationSubmission: recall</span><span class="sxs-lookup"><span data-stu-id="e1f06-104">educationSubmission: recall</span></span>

> <span data-ttu-id="e1f06-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e1f06-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1f06-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e1f06-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1f06-107">Indica que um estudante deseja reassumir o envio de um.</span><span class="sxs-lookup"><span data-stu-id="e1f06-107">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="e1f06-108">Essa ação só pode ser feita por um estudante.</span><span class="sxs-lookup"><span data-stu-id="e1f06-108">This action can only be done by a student.</span></span> <span data-ttu-id="e1f06-109">Ele alterará o status do envio de "enviado" Voltar ao "trabalho".</span><span class="sxs-lookup"><span data-stu-id="e1f06-109">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="e1f06-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1f06-110">Permissions</span></span>
<span data-ttu-id="e1f06-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1f06-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1f06-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1f06-113">Permission type</span></span>      | <span data-ttu-id="e1f06-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1f06-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1f06-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1f06-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="e1f06-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1f06-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e1f06-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1f06-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e1f06-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1f06-118">Not supported</span></span>  |
|<span data-ttu-id="e1f06-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1f06-119">Application</span></span> |<span data-ttu-id="e1f06-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1f06-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="e1f06-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1f06-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="e1f06-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1f06-122">Request headers</span></span>
| <span data-ttu-id="e1f06-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1f06-123">Header</span></span>       | <span data-ttu-id="e1f06-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e1f06-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1f06-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1f06-125">Authorization</span></span>  | <span data-ttu-id="e1f06-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1f06-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1f06-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1f06-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e1f06-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1f06-129">Response</span></span>
<span data-ttu-id="e1f06-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1f06-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1f06-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1f06-132">Example</span></span>
<span data-ttu-id="e1f06-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e1f06-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e1f06-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1f06-134">Request</span></span>
<span data-ttu-id="e1f06-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1f06-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="e1f06-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1f06-136">Response</span></span>
<span data-ttu-id="e1f06-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1f06-137">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->