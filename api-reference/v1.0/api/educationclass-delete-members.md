---
title: Remover um aluno
description: Remove um educationUser de uma educationClass
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: d5d0a51f7687c0ccab6da1a85dd5407faf08fd50
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883850"
---
# <a name="remove-a-student"></a><span data-ttu-id="8eac8-103">Remover um aluno</span><span class="sxs-lookup"><span data-stu-id="8eac8-103">Remove a student</span></span>

<span data-ttu-id="8eac8-104">Remove um [educationUser](../resources/educationuser.md) de uma [educationClass](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="8eac8-104">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="8eac8-105">**Observação:** professores _e_ alunos estão na coleção **members** da aula.</span><span class="sxs-lookup"><span data-stu-id="8eac8-105">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="8eac8-106">Antes de chamar essa API, garanta que **educationUser** que você está removendo não seja um professor.</span><span class="sxs-lookup"><span data-stu-id="8eac8-106">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="8eac8-107">Obtenha a lista de professores chamando [educationclass_list_teachers](educationclass-list-teachers.md) e verificando se a ID do usuário a ser removido não está na lista de professores retornada.</span><span class="sxs-lookup"><span data-stu-id="8eac8-107">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="8eac8-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8eac8-108">Permissions</span></span>
<span data-ttu-id="8eac8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eac8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eac8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8eac8-111">Permission type</span></span>      | <span data-ttu-id="8eac8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8eac8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8eac8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8eac8-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="8eac8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8eac8-114">Not supported.</span></span>  |
|<span data-ttu-id="8eac8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8eac8-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8eac8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8eac8-116">Not supported.</span></span>  |
|<span data-ttu-id="8eac8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8eac8-117">Application</span></span> | <span data-ttu-id="8eac8-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eac8-118">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8eac8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8eac8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8eac8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8eac8-120">Request headers</span></span>
| <span data-ttu-id="8eac8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8eac8-121">Header</span></span>       | <span data-ttu-id="8eac8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8eac8-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8eac8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8eac8-123">Authorization</span></span>  | <span data-ttu-id="8eac8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8eac8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8eac8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8eac8-126">Request body</span></span>
<span data-ttu-id="8eac8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8eac8-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8eac8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8eac8-128">Response</span></span>
<span data-ttu-id="8eac8-129">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="8eac8-129">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eac8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8eac8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8eac8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8eac8-131">Request</span></span>
<span data-ttu-id="8eac8-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8eac8-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/{member-id}
```

##### <a name="response"></a><span data-ttu-id="8eac8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8eac8-133">Response</span></span>
<span data-ttu-id="8eac8-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8eac8-134">The following is an example of the response.</span></span> 
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
