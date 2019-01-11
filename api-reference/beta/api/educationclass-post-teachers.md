---
title: Adicionar professor
description: Adicione um professor a uma aula.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 284c84cc140f0f9c15831396ed5adddaff73fdc6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882982"
---
# <a name="add-teacher"></a><span data-ttu-id="cfe1d-103">Adicionar professor</span><span class="sxs-lookup"><span data-stu-id="cfe1d-103">Add teacher</span></span>

> <span data-ttu-id="cfe1d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cfe1d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfe1d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cfe1d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cfe1d-106">Adicione um professor a uma aula.</span><span class="sxs-lookup"><span data-stu-id="cfe1d-106">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfe1d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cfe1d-107">Permissions</span></span>
<span data-ttu-id="cfe1d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfe1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfe1d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfe1d-110">Permission type</span></span>      | <span data-ttu-id="cfe1d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cfe1d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfe1d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfe1d-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="cfe1d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfe1d-113">Not supported.</span></span>  |
|<span data-ttu-id="cfe1d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfe1d-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cfe1d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfe1d-115">Not supported.</span></span>  |
|<span data-ttu-id="cfe1d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfe1d-116">Application</span></span> | <span data-ttu-id="cfe1d-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfe1d-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cfe1d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfe1d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="cfe1d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfe1d-119">Request headers</span></span>
| <span data-ttu-id="cfe1d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfe1d-120">Header</span></span>       | <span data-ttu-id="cfe1d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cfe1d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cfe1d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfe1d-122">Authorization</span></span>  | <span data-ttu-id="cfe1d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfe1d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cfe1d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cfe1d-125">Content-Type</span></span>  | <span data-ttu-id="cfe1d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cfe1d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cfe1d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfe1d-127">Request body</span></span>
<span data-ttu-id="cfe1d-128">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="cfe1d-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="cfe1d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfe1d-129">Response</span></span>
<span data-ttu-id="cfe1d-130">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfe1d-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfe1d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfe1d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cfe1d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfe1d-132">Request</span></span>
<span data-ttu-id="cfe1d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfe1d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11017/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14011"
}
```

##### <a name="response"></a><span data-ttu-id="cfe1d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfe1d-134">Response</span></span>
<span data-ttu-id="cfe1d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfe1d-135">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="cfe1d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfe1d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
