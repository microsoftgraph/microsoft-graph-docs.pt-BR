---
title: Criar synchronizationtemplate
description: Criar um novo modelo de sincronização para um determinado aplicativo.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f1477643bec6d7ca70eaec1a0c9ba000ff93db1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087877"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="66845-103">Criar synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="66845-103">Create synchronizationTemplate</span></span>

<span data-ttu-id="66845-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66845-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66845-105">Criar um novo modelo de sincronização para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66845-105">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="66845-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="66845-106">Permissions</span></span>
<span data-ttu-id="66845-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66845-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66845-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66845-109">Permission type</span></span>                        | <span data-ttu-id="66845-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66845-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="66845-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66845-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="66845-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66845-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="66845-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66845-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="66845-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66845-114">Not supported.</span></span>|
|<span data-ttu-id="66845-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66845-115">Application</span></span>                            |<span data-ttu-id="66845-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66845-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="66845-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66845-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="66845-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66845-118">Request headers</span></span>

| <span data-ttu-id="66845-119">Nome</span><span class="sxs-lookup"><span data-stu-id="66845-119">Name</span></span>           | <span data-ttu-id="66845-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="66845-120">Type</span></span>    | <span data-ttu-id="66845-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="66845-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="66845-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="66845-122">Authorization</span></span>  | <span data-ttu-id="66845-123">string</span><span class="sxs-lookup"><span data-stu-id="66845-123">string</span></span>  | <span data-ttu-id="66845-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66845-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66845-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66845-126">Request body</span></span>

<span data-ttu-id="66845-127">No corpo da solicitação, forneça o objeto [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) a ser criado.</span><span class="sxs-lookup"><span data-stu-id="66845-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="66845-128">As `id` `applicationId` Propriedades, e `factoryTag` são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="66845-128">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="66845-129">Quando o não `schema` é fornecido com o modelo, o esquema padrão associado à `factoryTag` propriedade será usado.</span><span class="sxs-lookup"><span data-stu-id="66845-129">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="66845-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="66845-130">Response</span></span>

<span data-ttu-id="66845-131">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66845-131">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="66845-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66845-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="66845-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66845-133">Request</span></span>
<span data-ttu-id="66845-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="66845-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66845-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="66845-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="66845-136">C#</span><span class="sxs-lookup"><span data-stu-id="66845-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationtemplate-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66845-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66845-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationtemplate-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66845-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66845-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationtemplate-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="66845-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="66845-139">Response</span></span>
<span data-ttu-id="66845-140">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="66845-140">The following is an example of a response.</span></span>
><span data-ttu-id="66845-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="66845-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="66845-142">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66845-142">All the properties will be returned in an actual call.</span></span>
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


