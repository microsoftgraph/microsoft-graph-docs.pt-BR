---
title: Excluir educationAssignmentResource
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c8154cc9112d62b06d2a93366f01fba3ea7907f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979583"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="8a47e-103">Excluir educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="8a47e-103">Delete educationAssignmentResource</span></span>

> <span data-ttu-id="8a47e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8a47e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a47e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8a47e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a47e-106">Exclua um recurso de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="8a47e-106">Delete a resource from an assignment.</span></span> <span data-ttu-id="8a47e-107">Somente professores na classe podem remover um recurso.</span><span class="sxs-lookup"><span data-stu-id="8a47e-107">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="8a47e-108">Depois que uma atribuição tiver sido publicada aos alunos, professores não é possível remover os recursos que são marcados como "distributeToStudents".</span><span class="sxs-lookup"><span data-stu-id="8a47e-108">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="8a47e-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="8a47e-109">Permissions</span></span>
<span data-ttu-id="8a47e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a47e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a47e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a47e-112">Permission type</span></span>      | <span data-ttu-id="8a47e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a47e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a47e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a47e-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="8a47e-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a47e-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8a47e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a47e-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8a47e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a47e-117">Not supported.</span></span>  |
|<span data-ttu-id="8a47e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a47e-118">Application</span></span> | <span data-ttu-id="8a47e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a47e-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8a47e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a47e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="8a47e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a47e-121">Request headers</span></span>
| <span data-ttu-id="8a47e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a47e-122">Header</span></span>       | <span data-ttu-id="8a47e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8a47e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a47e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a47e-124">Authorization</span></span>  | <span data-ttu-id="8a47e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a47e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a47e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a47e-127">Request body</span></span>
<span data-ttu-id="8a47e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a47e-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8a47e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a47e-129">Response</span></span>
<span data-ttu-id="8a47e-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a47e-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a47e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a47e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a47e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a47e-133">Request</span></span>
<span data-ttu-id="8a47e-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a47e-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="8a47e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a47e-135">Response</span></span>
<span data-ttu-id="8a47e-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8a47e-136">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
