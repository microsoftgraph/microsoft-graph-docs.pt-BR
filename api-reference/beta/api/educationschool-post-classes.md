---
title: Adicionar educationClass a educationSchool
description: Adicione uma aula a uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0ee3d1ba1a0b0da143ab3dbab5624d0ebb3de4ac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926208"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="da8bc-103">Adicionar educationClass a educationSchool</span><span class="sxs-lookup"><span data-stu-id="da8bc-103">Add educationClass to educationSchool</span></span>

> <span data-ttu-id="da8bc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da8bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da8bc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da8bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da8bc-106">Adicione uma aula a uma escola.</span><span class="sxs-lookup"><span data-stu-id="da8bc-106">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="da8bc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="da8bc-107">Permissions</span></span>
<span data-ttu-id="da8bc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da8bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da8bc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da8bc-110">Permission type</span></span>      | <span data-ttu-id="da8bc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da8bc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da8bc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da8bc-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="da8bc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da8bc-113">Not supported.</span></span>  |
|<span data-ttu-id="da8bc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da8bc-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="da8bc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da8bc-115">Not supported.</span></span>  |
|<span data-ttu-id="da8bc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da8bc-116">Application</span></span> | <span data-ttu-id="da8bc-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da8bc-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="da8bc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da8bc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="da8bc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da8bc-119">Request headers</span></span>
| <span data-ttu-id="da8bc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da8bc-120">Header</span></span>       | <span data-ttu-id="da8bc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="da8bc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da8bc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="da8bc-122">Authorization</span></span>  | <span data-ttu-id="da8bc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da8bc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da8bc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da8bc-125">Content-Type</span></span>  | <span data-ttu-id="da8bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da8bc-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da8bc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da8bc-127">Request body</span></span>
<span data-ttu-id="da8bc-128">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="da8bc-128">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="da8bc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="da8bc-129">Response</span></span>
<span data-ttu-id="da8bc-130">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da8bc-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da8bc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da8bc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da8bc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da8bc-132">Request</span></span>
<span data-ttu-id="da8bc-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="da8bc-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools/10002/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/beta/education/classes/11006"
}
```

##### <a name="response"></a><span data-ttu-id="da8bc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="da8bc-134">Response</span></span> 
<span data-ttu-id="da8bc-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="da8bc-135">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

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
