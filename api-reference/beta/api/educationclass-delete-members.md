---
title: Remover um aluno
description: Remove um educationUser de uma educationClass
author: mmast-msft
ms.openlocfilehash: 39defb72f4b0d01171ff92730a8e86b24c43a8ae
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348136"
---
# <a name="remove-a-student"></a><span data-ttu-id="8a1ae-103">Remover um aluno</span><span class="sxs-lookup"><span data-stu-id="8a1ae-103">Remove a student</span></span>

> <span data-ttu-id="8a1ae-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8a1ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a1ae-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8a1ae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a1ae-106">Remove um [educationUser](../resources/educationuser.md) de uma [educationClass](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="8a1ae-106">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="8a1ae-107">**Observação:** professores _e_ alunos estão na coleção **members** da aula.</span><span class="sxs-lookup"><span data-stu-id="8a1ae-107">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="8a1ae-108">Antes de chamar essa API, garanta que **educationUser** que você está removendo não seja um professor.</span><span class="sxs-lookup"><span data-stu-id="8a1ae-108">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="8a1ae-109">Obtenha a lista de professores chamando [educationclass_list_teachers](educationclass-list-teachers.md) e verificando se a ID do usuário a ser removido não está na lista de professores retornada.</span><span class="sxs-lookup"><span data-stu-id="8a1ae-109">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a1ae-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a1ae-110">Permissions</span></span>
<span data-ttu-id="8a1ae-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a1ae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a1ae-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a1ae-113">Permission type</span></span>      | <span data-ttu-id="8a1ae-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a1ae-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a1ae-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a1ae-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="8a1ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a1ae-116">Not supported.</span></span>  |
|<span data-ttu-id="8a1ae-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a1ae-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8a1ae-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a1ae-118">Not supported.</span></span>  |
|<span data-ttu-id="8a1ae-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a1ae-119">Application</span></span> | <span data-ttu-id="8a1ae-120">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a1ae-120">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8a1ae-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a1ae-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8a1ae-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a1ae-122">Request headers</span></span>
| <span data-ttu-id="8a1ae-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a1ae-123">Header</span></span>       | <span data-ttu-id="8a1ae-124">Valor</span><span class="sxs-lookup"><span data-stu-id="8a1ae-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a1ae-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a1ae-125">Authorization</span></span>  | <span data-ttu-id="8a1ae-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a1ae-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a1ae-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a1ae-128">Request body</span></span>
<span data-ttu-id="8a1ae-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a1ae-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8a1ae-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a1ae-130">Response</span></span>
<span data-ttu-id="8a1ae-131">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="8a1ae-131">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a1ae-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a1ae-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a1ae-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a1ae-133">Request</span></span>
<span data-ttu-id="8a1ae-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a1ae-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="8a1ae-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a1ae-135">Response</span></span>
<span data-ttu-id="8a1ae-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8a1ae-136">The following is an example of the response.</span></span> 
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
