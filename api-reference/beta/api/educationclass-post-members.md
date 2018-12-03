---
title: Adicionar um aluno
description: Adicione um membro a uma aula.
ms.openlocfilehash: 0b748a924de1f882372c0117f94d0de06f64dbc9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034015"
---
# <a name="add-a-student"></a><span data-ttu-id="27565-103">Adicionar um aluno</span><span class="sxs-lookup"><span data-stu-id="27565-103">Add a student</span></span>

> <span data-ttu-id="27565-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="27565-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27565-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="27565-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27565-106">Adicione um membro a uma aula.</span><span class="sxs-lookup"><span data-stu-id="27565-106">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="27565-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="27565-107">Permissions</span></span>
<span data-ttu-id="27565-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27565-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27565-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27565-110">Permission type</span></span>      | <span data-ttu-id="27565-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27565-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27565-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27565-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="27565-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27565-113">Not supported.</span></span>  |
|<span data-ttu-id="27565-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27565-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="27565-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27565-115">Not supported.</span></span>  |
|<span data-ttu-id="27565-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27565-116">Application</span></span> | <span data-ttu-id="27565-117">EduRoster.ReadWrite.All plus Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="27565-117">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="27565-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27565-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="27565-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27565-119">Request headers</span></span>
| <span data-ttu-id="27565-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27565-120">Header</span></span>       | <span data-ttu-id="27565-121">Valor</span><span class="sxs-lookup"><span data-stu-id="27565-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27565-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27565-122">Authorization</span></span>  | <span data-ttu-id="27565-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27565-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="27565-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27565-125">Content-Type</span></span>  | <span data-ttu-id="27565-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27565-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27565-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27565-127">Request body</span></span>
<span data-ttu-id="27565-128">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="27565-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="27565-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="27565-129">Response</span></span>
<span data-ttu-id="27565-130">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27565-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27565-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27565-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27565-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27565-132">Request</span></span>
<span data-ttu-id="27565-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27565-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11011/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/13015"
}
```

##### <a name="response"></a><span data-ttu-id="27565-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="27565-134">Response</span></span>
<span data-ttu-id="27565-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27565-135">The following is an example of the response.</span></span> 


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
