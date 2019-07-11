---
title: Criar synchronizationtemplate
description: Criar um novo modelo de sincronização para um determinado aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1573d741acb0571784730ac6a37bc7b970e0cf3c
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620427"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="d6077-103">Criar synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="d6077-103">Create synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6077-104">Criar um novo modelo de sincronização para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d6077-104">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6077-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6077-105">Permissions</span></span>
<span data-ttu-id="d6077-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6077-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6077-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6077-108">Permission type</span></span>                        | <span data-ttu-id="d6077-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6077-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6077-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6077-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="d6077-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6077-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="d6077-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6077-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d6077-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6077-113">Not supported.</span></span>|
|<span data-ttu-id="d6077-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6077-114">Application</span></span>                            |<span data-ttu-id="d6077-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6077-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="d6077-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6077-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="d6077-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6077-117">Request headers</span></span>

| <span data-ttu-id="d6077-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d6077-118">Name</span></span>           | <span data-ttu-id="d6077-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6077-119">Type</span></span>    | <span data-ttu-id="d6077-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6077-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="d6077-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6077-121">Authorization</span></span>  | <span data-ttu-id="d6077-122">string</span><span class="sxs-lookup"><span data-stu-id="d6077-122">string</span></span>  | <span data-ttu-id="d6077-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6077-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6077-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6077-125">Request body</span></span>

<span data-ttu-id="d6077-126">No corpo da solicitação, forneça o [](../resources/synchronization-synchronizationtemplate.md) objeto synchronizationtemplate a ser criado.</span><span class="sxs-lookup"><span data-stu-id="d6077-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="d6077-127">As `id`propriedades `applicationId` , `factoryTag` e são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="d6077-127">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="d6077-128">Quando o `schema` não é fornecido com o modelo, o esquema padrão associado à `factoryTag` propriedade será usado.</span><span class="sxs-lookup"><span data-stu-id="d6077-128">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="d6077-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6077-129">Response</span></span>

<span data-ttu-id="d6077-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6077-130">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="d6077-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6077-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d6077-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6077-132">Request</span></span>
<span data-ttu-id="d6077-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6077-133">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d6077-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6077-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/synchronization/templates
Content-type: application/json

{ 
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6077-135">C#</span><span class="sxs-lookup"><span data-stu-id="d6077-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationtemplate-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6077-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6077-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationtemplate-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6077-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d6077-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationtemplate-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d6077-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6077-138">Response</span></span>
<span data-ttu-id="d6077-139">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="d6077-139">The following is an example of a response.</span></span>
><span data-ttu-id="d6077-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d6077-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d6077-141">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6077-141">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 201 Created

{
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
