---
title: 'educationSubmission: versão'
description: " e indica que a classificação é feita. Essa ação só pode ser feita com o professor."
author: dipakboyed
ms.openlocfilehash: 9a21c45198ccd0ef933d58721c2d594cf29443bc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308586"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="5c280-104">educationSubmission: versão</span><span class="sxs-lookup"><span data-stu-id="5c280-104">educationSubmission: release</span></span>

> <span data-ttu-id="5c280-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5c280-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c280-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5c280-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c280-107">Esta ação faz com que o nível e os comentários associados a esse envio disponível ao aluno.</span><span class="sxs-lookup"><span data-stu-id="5c280-107">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="5c280-108">Isso irá alterar o status do envio de "enviado" para "liberados" e indica que a classificação é feita.</span><span class="sxs-lookup"><span data-stu-id="5c280-108">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="5c280-109">Essa ação só pode ser feita com o professor.</span><span class="sxs-lookup"><span data-stu-id="5c280-109">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c280-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c280-110">Permissions</span></span>
<span data-ttu-id="5c280-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c280-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c280-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c280-113">Permission type</span></span>      | <span data-ttu-id="5c280-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c280-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c280-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c280-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="5c280-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c280-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="5c280-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c280-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5c280-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c280-118">Not supported.</span></span>  |
|<span data-ttu-id="5c280-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c280-119">Application</span></span> | <span data-ttu-id="5c280-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c280-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5c280-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c280-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="5c280-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c280-122">Request headers</span></span>
| <span data-ttu-id="5c280-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c280-123">Header</span></span>       | <span data-ttu-id="5c280-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5c280-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5c280-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c280-125">Authorization</span></span>  | <span data-ttu-id="5c280-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c280-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5c280-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c280-128">Request body</span></span>
<span data-ttu-id="5c280-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c280-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c280-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c280-130">Response</span></span>
<span data-ttu-id="5c280-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c280-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c280-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c280-133">Example</span></span>
<span data-ttu-id="5c280-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5c280-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5c280-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c280-135">Request</span></span>
<span data-ttu-id="5c280-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c280-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="5c280-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c280-137">Response</span></span>
<span data-ttu-id="5c280-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c280-138">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: release",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->