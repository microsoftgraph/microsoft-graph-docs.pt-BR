---
title: Remover professor
description: Remova um professor de uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 35151136f38bcf1e74d958f3f48f4e6819ab73cf
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750014"
---
# <a name="remove-teacher"></a><span data-ttu-id="25f0f-103">Remover professor</span><span class="sxs-lookup"><span data-stu-id="25f0f-103">Remove teacher</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25f0f-104">Remova um professor de uma aula.</span><span class="sxs-lookup"><span data-stu-id="25f0f-104">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="25f0f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="25f0f-105">Permissions</span></span>

<span data-ttu-id="25f0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25f0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25f0f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25f0f-108">Permission type</span></span>                        | <span data-ttu-id="25f0f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25f0f-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="25f0f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25f0f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="25f0f-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25f0f-111">Not supported.</span></span>                              |
| <span data-ttu-id="25f0f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25f0f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25f0f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25f0f-113">Not supported.</span></span>                              |
| <span data-ttu-id="25f0f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25f0f-114">Application</span></span>                            | <span data-ttu-id="25f0f-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25f0f-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="25f0f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25f0f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="25f0f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25f0f-117">Request headers</span></span>

| <span data-ttu-id="25f0f-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25f0f-118">Header</span></span>        | <span data-ttu-id="25f0f-119">Valor</span><span class="sxs-lookup"><span data-stu-id="25f0f-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="25f0f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="25f0f-120">Authorization</span></span> | <span data-ttu-id="25f0f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25f0f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25f0f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25f0f-123">Request body</span></span>

<span data-ttu-id="25f0f-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25f0f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25f0f-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="25f0f-125">Response</span></span>

<span data-ttu-id="25f0f-126">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="25f0f-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="25f0f-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25f0f-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="25f0f-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25f0f-128">Request</span></span>

<span data-ttu-id="25f0f-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="25f0f-129">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/{id}/teachers/14012
```

##### <a name="response"></a><span data-ttu-id="25f0f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="25f0f-130">Response</span></span>

<span data-ttu-id="25f0f-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="25f0f-131">The following is an example of the response.</span></span> 

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
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
