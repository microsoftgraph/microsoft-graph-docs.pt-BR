---
title: Criar synchronizationtemplate
description: Criar um novo modelo de sincronização para um determinado aplicativo.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4f612065222a43e67ea82101519b44bad1604c53
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363383"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="50518-103">Criar synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="50518-103">Create synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50518-104">Criar um novo modelo de sincronização para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50518-104">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="50518-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="50518-105">Permissions</span></span>
<span data-ttu-id="50518-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50518-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50518-108">Permission type</span></span>                        | <span data-ttu-id="50518-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50518-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="50518-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50518-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="50518-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50518-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="50518-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50518-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="50518-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50518-113">Not supported.</span></span>|
|<span data-ttu-id="50518-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50518-114">Application</span></span>                            |<span data-ttu-id="50518-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50518-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="50518-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50518-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="50518-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50518-117">Request headers</span></span>

| <span data-ttu-id="50518-118">Nome</span><span class="sxs-lookup"><span data-stu-id="50518-118">Name</span></span>           | <span data-ttu-id="50518-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="50518-119">Type</span></span>    | <span data-ttu-id="50518-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="50518-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="50518-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="50518-121">Authorization</span></span>  | <span data-ttu-id="50518-122">string</span><span class="sxs-lookup"><span data-stu-id="50518-122">string</span></span>  | <span data-ttu-id="50518-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50518-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50518-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50518-125">Request body</span></span>

<span data-ttu-id="50518-126">No corpo da solicitação, forneça o [](../resources/synchronization-synchronizationtemplate.md) objeto synchronizationtemplate a ser criado.</span><span class="sxs-lookup"><span data-stu-id="50518-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="50518-127">As `id`propriedades `applicationId` , `factoryTag` e são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="50518-127">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="50518-128">Quando o `schema` não é fornecido com o modelo, o esquema padrão associado à `factoryTag` propriedade será usado.</span><span class="sxs-lookup"><span data-stu-id="50518-128">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="50518-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="50518-129">Response</span></span>

<span data-ttu-id="50518-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50518-130">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="50518-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50518-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="50518-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50518-132">Request</span></span>
<span data-ttu-id="50518-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="50518-133">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="50518-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="50518-134">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="50518-135">C#</span><span class="sxs-lookup"><span data-stu-id="50518-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationtemplate-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50518-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50518-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationtemplate-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="50518-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="50518-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationtemplate-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="50518-138">Java</span><span class="sxs-lookup"><span data-stu-id="50518-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-synchronizationtemplate-from-synchronization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="50518-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="50518-139">Response</span></span>
<span data-ttu-id="50518-140">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="50518-140">The following is an example of a response.</span></span>
><span data-ttu-id="50518-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="50518-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="50518-142">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50518-142">All the properties will be returned in an actual call.</span></span>
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
