---
title: Excluir educationSubmissionResource
description: " o recurso ao seu estado original. Se o recurso não foi copiado da atribuição, mas foi adicionado de student, o recurso simplesmente é excluído."
ms.openlocfilehash: 9eb5b08e2e5481e707cc6c1e0b0f8339e3d22ad4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038095"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="3130c-104">Excluir educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="3130c-104">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="3130c-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3130c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3130c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3130c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3130c-107">Exclui um recurso do envio.</span><span class="sxs-lookup"><span data-stu-id="3130c-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="3130c-108">Isso só pode ser feito pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="3130c-108">This can only be done by the student.</span></span> <span data-ttu-id="3130c-109">Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada depois que a cópia atual for excluída.</span><span class="sxs-lookup"><span data-stu-id="3130c-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="3130c-110">Isso permite "Redefinir" o recurso ao seu estado original.</span><span class="sxs-lookup"><span data-stu-id="3130c-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="3130c-111">Se o recurso não foi copiado da atribuição, mas foi adicionado de student, o recurso simplesmente é excluído.</span><span class="sxs-lookup"><span data-stu-id="3130c-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="3130c-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="3130c-112">Permissions</span></span>
<span data-ttu-id="3130c-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3130c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3130c-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3130c-115">Permission type</span></span>      | <span data-ttu-id="3130c-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3130c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3130c-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3130c-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="3130c-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3130c-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="3130c-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3130c-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3130c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3130c-120">Not supported.</span></span>  |
|<span data-ttu-id="3130c-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3130c-121">Application</span></span> | <span data-ttu-id="3130c-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3130c-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3130c-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3130c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3130c-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3130c-124">Request headers</span></span>
| <span data-ttu-id="3130c-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3130c-125">Header</span></span>       | <span data-ttu-id="3130c-126">Valor</span><span class="sxs-lookup"><span data-stu-id="3130c-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3130c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="3130c-127">Authorization</span></span>  | <span data-ttu-id="3130c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3130c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3130c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3130c-130">Request body</span></span>
<span data-ttu-id="3130c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3130c-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3130c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3130c-132">Response</span></span>
<span data-ttu-id="3130c-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3130c-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3130c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3130c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3130c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3130c-136">Request</span></span>
<span data-ttu-id="3130c-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3130c-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="3130c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3130c-138">Response</span></span>
<span data-ttu-id="3130c-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3130c-139">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->