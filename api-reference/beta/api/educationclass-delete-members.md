---
title: Remover um aluno
description: Remove um educationUser de uma educationClass
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ba9d490691b6d717fc1d088408c25a2724eb491a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457946"
---
# <a name="remove-a-student"></a><span data-ttu-id="a81d6-103">Remover um aluno</span><span class="sxs-lookup"><span data-stu-id="a81d6-103">Remove a student</span></span>

<span data-ttu-id="a81d6-104">Remove um [educationUser](../resources/educationuser.md) de uma [educationClass](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="a81d6-104">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="a81d6-105">**Observação:** professores _e_ alunos estão na coleção **members** da aula.</span><span class="sxs-lookup"><span data-stu-id="a81d6-105">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="a81d6-106">Antes de chamar essa API, garanta que **educationUser** que você está removendo não seja um professor.</span><span class="sxs-lookup"><span data-stu-id="a81d6-106">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="a81d6-107">Obtenha a lista de professores chamando [educationclass_list_teachers](educationclass-list-teachers.md) e verificando se a ID do usuário a ser removido não está na lista de professores retornada.</span><span class="sxs-lookup"><span data-stu-id="a81d6-107">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="a81d6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a81d6-108">Permissions</span></span>
<span data-ttu-id="a81d6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a81d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a81d6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a81d6-111">Permission type</span></span>      | <span data-ttu-id="a81d6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a81d6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a81d6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a81d6-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="a81d6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a81d6-114">Not supported.</span></span>  |
|<span data-ttu-id="a81d6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a81d6-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a81d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a81d6-116">Not supported.</span></span>  |
|<span data-ttu-id="a81d6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a81d6-117">Application</span></span> | <span data-ttu-id="a81d6-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a81d6-118">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a81d6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a81d6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a81d6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a81d6-120">Request headers</span></span>
| <span data-ttu-id="a81d6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a81d6-121">Header</span></span>       | <span data-ttu-id="a81d6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a81d6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a81d6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a81d6-123">Authorization</span></span>  | <span data-ttu-id="a81d6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a81d6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a81d6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a81d6-126">Request body</span></span>
<span data-ttu-id="a81d6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a81d6-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a81d6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a81d6-128">Response</span></span>
<span data-ttu-id="a81d6-129">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="a81d6-129">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="a81d6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a81d6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a81d6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a81d6-131">Request</span></span>
<span data-ttu-id="a81d6-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a81d6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/{member-id}
```

##### <a name="response"></a><span data-ttu-id="a81d6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a81d6-133">Response</span></span>
<span data-ttu-id="a81d6-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a81d6-134">The following is an example of the response.</span></span> 
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
