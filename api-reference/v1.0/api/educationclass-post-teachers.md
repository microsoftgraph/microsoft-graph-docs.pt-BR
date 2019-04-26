---
title: Adicionar professor
description: Adicione um professor a uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a8c968890877ec07112510615b11010efb3779a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550473"
---
# <a name="add-teacher"></a><span data-ttu-id="f85cd-103">Adicionar professor</span><span class="sxs-lookup"><span data-stu-id="f85cd-103">Add teacher</span></span>

<span data-ttu-id="f85cd-104">Adicione um professor a uma aula.</span><span class="sxs-lookup"><span data-stu-id="f85cd-104">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="f85cd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f85cd-105">Permissions</span></span>
<span data-ttu-id="f85cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f85cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f85cd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f85cd-108">Permission type</span></span>      | <span data-ttu-id="f85cd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f85cd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f85cd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f85cd-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f85cd-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f85cd-111">Not supported.</span></span>  |
|<span data-ttu-id="f85cd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f85cd-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f85cd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f85cd-113">Not supported.</span></span>  |
|<span data-ttu-id="f85cd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f85cd-114">Application</span></span> | <span data-ttu-id="f85cd-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f85cd-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f85cd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f85cd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f85cd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f85cd-117">Request headers</span></span>
| <span data-ttu-id="f85cd-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f85cd-118">Header</span></span>       | <span data-ttu-id="f85cd-119">Valor</span><span class="sxs-lookup"><span data-stu-id="f85cd-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f85cd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f85cd-120">Authorization</span></span>  | <span data-ttu-id="f85cd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f85cd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f85cd-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f85cd-123">Content-Type</span></span>  | <span data-ttu-id="f85cd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f85cd-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f85cd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f85cd-125">Request body</span></span>
<span data-ttu-id="f85cd-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="f85cd-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="f85cd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f85cd-127">Response</span></span>
<span data-ttu-id="f85cd-128">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f85cd-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f85cd-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f85cd-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f85cd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f85cd-130">Request</span></span>
<span data-ttu-id="f85cd-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f85cd-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14011"
}
```

##### <a name="response"></a><span data-ttu-id="f85cd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f85cd-132">Response</span></span>
<span data-ttu-id="f85cd-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f85cd-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="f85cd-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f85cd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
