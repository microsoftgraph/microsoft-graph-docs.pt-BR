---
title: Remover educationClass
description: Exclua uma classe de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a1ae6e96358f0ea6c85feb8cfec50a68ba1a7ee4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934972"
---
# <a name="remove-educationclass"></a><span data-ttu-id="df184-103">Remover educationClass</span><span class="sxs-lookup"><span data-stu-id="df184-103">Remove educationClass</span></span>

> <span data-ttu-id="df184-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="df184-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df184-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="df184-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df184-106">Exclua uma classe de uma escola.</span><span class="sxs-lookup"><span data-stu-id="df184-106">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="df184-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="df184-107">Permissions</span></span>
<span data-ttu-id="df184-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df184-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df184-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df184-110">Permission type</span></span>      | <span data-ttu-id="df184-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df184-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df184-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df184-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="df184-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df184-113">Not supported.</span></span>  |
|<span data-ttu-id="df184-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df184-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="df184-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df184-115">Not supported.</span></span>  |
|<span data-ttu-id="df184-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df184-116">Application</span></span> | <span data-ttu-id="df184-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df184-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="df184-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df184-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="df184-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df184-119">Request headers</span></span>
| <span data-ttu-id="df184-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df184-120">Header</span></span>       | <span data-ttu-id="df184-121">Valor</span><span class="sxs-lookup"><span data-stu-id="df184-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df184-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df184-122">Authorization</span></span>  | <span data-ttu-id="df184-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df184-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df184-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df184-125">Request body</span></span>
<span data-ttu-id="df184-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df184-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="df184-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="df184-127">Response</span></span>
<span data-ttu-id="df184-128">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df184-128">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="df184-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df184-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df184-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df184-130">Request</span></span>
<span data-ttu-id="df184-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df184-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="df184-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="df184-132">Response</span></span>
<span data-ttu-id="df184-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df184-133">The following is an example of the response.</span></span> 

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
