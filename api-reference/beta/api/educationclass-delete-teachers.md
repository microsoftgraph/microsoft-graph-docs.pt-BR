---
title: Remover professor
description: Remova um professor de uma aula.
ms.openlocfilehash: bc472704d5a8184775f755505da497be4b825265
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034636"
---
# <a name="remove-teacher"></a><span data-ttu-id="4865f-103">Remover professor</span><span class="sxs-lookup"><span data-stu-id="4865f-103">Remove teacher</span></span>

> <span data-ttu-id="4865f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4865f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4865f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4865f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4865f-106">Remova um professor de uma aula.</span><span class="sxs-lookup"><span data-stu-id="4865f-106">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="4865f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4865f-107">Permissions</span></span>
<span data-ttu-id="4865f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4865f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4865f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4865f-110">Permission type</span></span>      | <span data-ttu-id="4865f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4865f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4865f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4865f-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="4865f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4865f-113">Not supported.</span></span>  |
|<span data-ttu-id="4865f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4865f-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4865f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4865f-115">Not supported.</span></span>  |
|<span data-ttu-id="4865f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4865f-116">Application</span></span> | <span data-ttu-id="4865f-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4865f-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4865f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4865f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4865f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4865f-119">Request headers</span></span>
| <span data-ttu-id="4865f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4865f-120">Header</span></span>       | <span data-ttu-id="4865f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4865f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4865f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4865f-122">Authorization</span></span>  | <span data-ttu-id="4865f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4865f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4865f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4865f-125">Request body</span></span>
<span data-ttu-id="4865f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4865f-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4865f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4865f-127">Response</span></span>
<span data-ttu-id="4865f-128">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="4865f-128">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="4865f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4865f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4865f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4865f-130">Request</span></span>
<span data-ttu-id="4865f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4865f-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/<id>/teachers/14012
```

##### <a name="response"></a><span data-ttu-id="4865f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4865f-132">Response</span></span>
<span data-ttu-id="4865f-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4865f-133">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
