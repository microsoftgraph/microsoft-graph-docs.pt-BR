---
title: Adicionar educationUser a uma educationSchool
description: Adicione um usuário a uma escola.
author: mmast-msft
ms.openlocfilehash: 4c77a94b7b1c9af11d954a4ab903c597eded6a04
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352726"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="ce28e-103">Adicionar educationUser a uma educationSchool</span><span class="sxs-lookup"><span data-stu-id="ce28e-103">Add educationUser to an educationSchool</span></span>

> <span data-ttu-id="ce28e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ce28e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce28e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ce28e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce28e-106">Adicione um usuário a uma escola.</span><span class="sxs-lookup"><span data-stu-id="ce28e-106">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce28e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce28e-107">Permissions</span></span>
<span data-ttu-id="ce28e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce28e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce28e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce28e-110">Permission type</span></span>      | <span data-ttu-id="ce28e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce28e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce28e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce28e-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="ce28e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce28e-113">Not supported.</span></span>  |
|<span data-ttu-id="ce28e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce28e-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ce28e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce28e-115">Not supported.</span></span>  |
|<span data-ttu-id="ce28e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce28e-116">Application</span></span> | <span data-ttu-id="ce28e-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce28e-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ce28e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce28e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ce28e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce28e-119">Request headers</span></span>
| <span data-ttu-id="ce28e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce28e-120">Header</span></span>       | <span data-ttu-id="ce28e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ce28e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce28e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce28e-122">Authorization</span></span>  | <span data-ttu-id="ce28e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce28e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ce28e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce28e-125">Content-Type</span></span>  | <span data-ttu-id="ce28e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce28e-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ce28e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce28e-127">Request body</span></span>
<span data-ttu-id="ce28e-128">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="ce28e-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ce28e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce28e-129">Response</span></span>
<span data-ttu-id="ce28e-130">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce28e-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce28e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce28e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce28e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce28e-132">Request</span></span>
<span data-ttu-id="ce28e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce28e-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools/<id>/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14008"
}
```

##### <a name="response"></a><span data-ttu-id="ce28e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce28e-134">Response</span></span>
<span data-ttu-id="ce28e-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce28e-135">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->