---
title: Excluir educationSubmissionResource
description: Exclui um recurso do envio. Isso só pode ser feito pelo aluno. Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada depois que a cópia atual for excluída.
author: dipakboyed
ms.openlocfilehash: d56df6cee3884556186554d9c24ae09ed802c4f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313269"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="dbe5a-105">Excluir educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="dbe5a-105">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="dbe5a-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbe5a-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbe5a-108">Exclui um recurso do envio.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-108">Deletes a resource from the submission.</span></span> <span data-ttu-id="dbe5a-109">Isso só pode ser feito pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-109">This can only be done by the student.</span></span> <span data-ttu-id="dbe5a-110">Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada depois que a cópia atual for excluída.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-110">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="dbe5a-111">Isso permite "Redefinir" o recurso ao seu estado original.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-111">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="dbe5a-112">Se o recurso não foi copiado da atribuição, mas foi adicionado de student, o recurso simplesmente é excluído.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-112">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbe5a-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbe5a-113">Permissions</span></span>
<span data-ttu-id="dbe5a-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbe5a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbe5a-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbe5a-116">Permission type</span></span>      | <span data-ttu-id="dbe5a-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbe5a-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbe5a-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbe5a-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="dbe5a-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbe5a-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="dbe5a-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbe5a-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dbe5a-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-121">Not supported.</span></span>  |
|<span data-ttu-id="dbe5a-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbe5a-122">Application</span></span> | <span data-ttu-id="dbe5a-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dbe5a-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbe5a-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="dbe5a-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe5a-125">Request headers</span></span>
| <span data-ttu-id="dbe5a-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbe5a-126">Header</span></span>       | <span data-ttu-id="dbe5a-127">Valor</span><span class="sxs-lookup"><span data-stu-id="dbe5a-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dbe5a-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbe5a-128">Authorization</span></span>  | <span data-ttu-id="dbe5a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dbe5a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe5a-131">Request body</span></span>
<span data-ttu-id="dbe5a-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="dbe5a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbe5a-133">Response</span></span>
<span data-ttu-id="dbe5a-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbe5a-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbe5a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dbe5a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe5a-137">Request</span></span>
<span data-ttu-id="dbe5a-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="dbe5a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbe5a-139">Response</span></span>
<span data-ttu-id="dbe5a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dbe5a-140">The following is an example of the response.</span></span> 

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