---
title: Criar synchronizationTemplate
description: Crie um novo modelo de sincronização para um determinado aplicativo.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 054e5dfc672f3336e5c8d633e05c1db82e350fdd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137239"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="1a484-103">Criar synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="1a484-103">Create synchronizationTemplate</span></span>

<span data-ttu-id="1a484-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a484-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a484-105">Crie um novo modelo de sincronização para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1a484-105">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a484-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a484-106">Permissions</span></span>
<span data-ttu-id="1a484-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a484-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a484-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a484-109">Permission type</span></span>                        | <span data-ttu-id="1a484-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a484-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a484-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a484-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="1a484-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a484-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="1a484-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a484-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="1a484-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a484-114">Not supported.</span></span>|
|<span data-ttu-id="1a484-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a484-115">Application</span></span>                            |<span data-ttu-id="1a484-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a484-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="1a484-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a484-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="1a484-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a484-118">Request headers</span></span>

| <span data-ttu-id="1a484-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1a484-119">Name</span></span>           | <span data-ttu-id="1a484-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a484-120">Type</span></span>    | <span data-ttu-id="1a484-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a484-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="1a484-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a484-122">Authorization</span></span>  | <span data-ttu-id="1a484-123">string</span><span class="sxs-lookup"><span data-stu-id="1a484-123">string</span></span>  | <span data-ttu-id="1a484-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a484-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a484-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a484-126">Request body</span></span>

<span data-ttu-id="1a484-127">No corpo da solicitação, fornece o [objeto synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) a ser criado.</span><span class="sxs-lookup"><span data-stu-id="1a484-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="1a484-128">The `id` , and properties are `applicationId` `factoryTag` required.</span><span class="sxs-lookup"><span data-stu-id="1a484-128">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="1a484-129">Quando não for fornecido nenhum com o modelo, o esquema `schema` padrão associado à propriedade será `factoryTag` usado.</span><span class="sxs-lookup"><span data-stu-id="1a484-129">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="1a484-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a484-130">Response</span></span>

<span data-ttu-id="1a484-131">Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a484-131">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="1a484-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a484-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1a484-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a484-133">Request</span></span>
<span data-ttu-id="1a484-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a484-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a484-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a484-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1a484-136">C#</span><span class="sxs-lookup"><span data-stu-id="1a484-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationtemplate-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a484-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a484-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationtemplate-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a484-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a484-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationtemplate-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a484-139">Java</span><span class="sxs-lookup"><span data-stu-id="1a484-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-synchronizationtemplate-from-synchronization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1a484-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a484-140">Response</span></span>
<span data-ttu-id="1a484-141">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="1a484-141">The following is an example of a response.</span></span>
><span data-ttu-id="1a484-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1a484-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1a484-143">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a484-143">All the properties will be returned in an actual call.</span></span>
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


