---
title: Excluir educationSubmissionResource
description: Exclui um recurso do envio. Isso só pode ser feito pelo aluno. Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada depois que a cópia atual for excluída.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 94e73f7b4c6c0c0bc85b21ee3e651f8e61234e80
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828809"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="ddd4c-105">Excluir educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="ddd4c-105">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="ddd4c-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddd4c-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ddd4c-108">Exclui um recurso do envio.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-108">Deletes a resource from the submission.</span></span> <span data-ttu-id="ddd4c-109">Isso só pode ser feito pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-109">This can only be done by the student.</span></span> <span data-ttu-id="ddd4c-110">Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada depois que a cópia atual for excluída.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-110">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="ddd4c-111">Isso permite "Redefinir" o recurso ao seu estado original.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-111">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="ddd4c-112">Se o recurso não foi copiado da atribuição, mas foi adicionado de student, o recurso simplesmente é excluído.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-112">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddd4c-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="ddd4c-113">Permissions</span></span>
<span data-ttu-id="ddd4c-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddd4c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddd4c-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddd4c-116">Permission type</span></span>      | <span data-ttu-id="ddd4c-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddd4c-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddd4c-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddd4c-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="ddd4c-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddd4c-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ddd4c-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddd4c-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ddd4c-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-121">Not supported.</span></span>  |
|<span data-ttu-id="ddd4c-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddd4c-122">Application</span></span> | <span data-ttu-id="ddd4c-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ddd4c-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddd4c-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ddd4c-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddd4c-125">Request headers</span></span>
| <span data-ttu-id="ddd4c-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ddd4c-126">Header</span></span>       | <span data-ttu-id="ddd4c-127">Valor</span><span class="sxs-lookup"><span data-stu-id="ddd4c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ddd4c-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddd4c-128">Authorization</span></span>  | <span data-ttu-id="ddd4c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ddd4c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddd4c-131">Request body</span></span>
<span data-ttu-id="ddd4c-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ddd4c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddd4c-133">Response</span></span>
<span data-ttu-id="ddd4c-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddd4c-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddd4c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ddd4c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddd4c-137">Request</span></span>
<span data-ttu-id="ddd4c-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="ddd4c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddd4c-139">Response</span></span>
<span data-ttu-id="ddd4c-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddd4c-140">The following is an example of the response.</span></span> 

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
