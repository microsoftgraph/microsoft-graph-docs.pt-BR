---
title: 'educationSubmission: recall'
description: .
ms.openlocfilehash: 8df134a6d8325e5b497baada89bc0fa16d0ee9e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033991"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="e4afc-103">educationSubmission: recall</span><span class="sxs-lookup"><span data-stu-id="e4afc-103">educationSubmission: recall</span></span>

> <span data-ttu-id="e4afc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e4afc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4afc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e4afc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4afc-106">Indica que um estudante deseja reassumir o envio de um.</span><span class="sxs-lookup"><span data-stu-id="e4afc-106">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="e4afc-107">Essa ação só pode ser feita por um estudante.</span><span class="sxs-lookup"><span data-stu-id="e4afc-107">This action can only be done by a student.</span></span> <span data-ttu-id="e4afc-108">Ele alterará o status do envio de "enviado" Voltar ao "trabalho".</span><span class="sxs-lookup"><span data-stu-id="e4afc-108">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="e4afc-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="e4afc-109">Permissions</span></span>
<span data-ttu-id="e4afc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4afc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4afc-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4afc-112">Permission type</span></span>      | <span data-ttu-id="e4afc-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4afc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4afc-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4afc-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="e4afc-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4afc-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e4afc-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4afc-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e4afc-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e4afc-117">Not supported</span></span>  |
|<span data-ttu-id="e4afc-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4afc-118">Application</span></span> |<span data-ttu-id="e4afc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4afc-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="e4afc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4afc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="e4afc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4afc-121">Request headers</span></span>
| <span data-ttu-id="e4afc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4afc-122">Header</span></span>       | <span data-ttu-id="e4afc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e4afc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e4afc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4afc-124">Authorization</span></span>  | <span data-ttu-id="e4afc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4afc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4afc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4afc-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e4afc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4afc-128">Response</span></span>
<span data-ttu-id="e4afc-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4afc-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4afc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4afc-131">Example</span></span>
<span data-ttu-id="e4afc-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e4afc-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e4afc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4afc-133">Request</span></span>
<span data-ttu-id="e4afc-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4afc-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="e4afc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4afc-135">Response</span></span>
<span data-ttu-id="e4afc-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4afc-136">The following is an example of the response.</span></span>

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