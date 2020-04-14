---
title: Criar synchronizationtemplate
description: Criar um novo modelo de sincronização para um determinado aplicativo.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b75d5e2f052983cab54fe1cdfd557e03b7778e6e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471135"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="2cbf6-103">Criar synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="2cbf6-103">Create synchronizationTemplate</span></span>

<span data-ttu-id="2cbf6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cbf6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cbf6-105">Criar um novo modelo de sincronização para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2cbf6-105">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cbf6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2cbf6-106">Permissions</span></span>
<span data-ttu-id="2cbf6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cbf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cbf6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2cbf6-109">Permission type</span></span>                        | <span data-ttu-id="2cbf6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2cbf6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cbf6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2cbf6-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="2cbf6-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cbf6-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="2cbf6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2cbf6-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="2cbf6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cbf6-114">Not supported.</span></span>|
|<span data-ttu-id="2cbf6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2cbf6-115">Application</span></span>                            |<span data-ttu-id="2cbf6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cbf6-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="2cbf6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2cbf6-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="2cbf6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2cbf6-118">Request headers</span></span>

| <span data-ttu-id="2cbf6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2cbf6-119">Name</span></span>           | <span data-ttu-id="2cbf6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cbf6-120">Type</span></span>    | <span data-ttu-id="2cbf6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cbf6-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="2cbf6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2cbf6-122">Authorization</span></span>  | <span data-ttu-id="2cbf6-123">string</span><span class="sxs-lookup"><span data-stu-id="2cbf6-123">string</span></span>  | <span data-ttu-id="2cbf6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cbf6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cbf6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2cbf6-126">Request body</span></span>

<span data-ttu-id="2cbf6-127">No corpo da solicitação, forneça o objeto [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) a ser criado.</span><span class="sxs-lookup"><span data-stu-id="2cbf6-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="2cbf6-128">As `id`propriedades `applicationId` , `factoryTag` e são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="2cbf6-128">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="2cbf6-129">Quando o `schema` não é fornecido com o modelo, o esquema padrão associado à `factoryTag` propriedade será usado.</span><span class="sxs-lookup"><span data-stu-id="2cbf6-129">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="2cbf6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cbf6-130">Response</span></span>

<span data-ttu-id="2cbf6-131">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2cbf6-131">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="2cbf6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2cbf6-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2cbf6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2cbf6-133">Request</span></span>
<span data-ttu-id="2cbf6-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="2cbf6-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2cbf6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cbf6-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2cbf6-136">C#</span><span class="sxs-lookup"><span data-stu-id="2cbf6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationtemplate-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cbf6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cbf6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationtemplate-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cbf6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cbf6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationtemplate-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2cbf6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cbf6-139">Response</span></span>
<span data-ttu-id="2cbf6-140">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="2cbf6-140">The following is an example of a response.</span></span>
><span data-ttu-id="2cbf6-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2cbf6-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2cbf6-142">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2cbf6-142">All the properties will be returned in an actual call.</span></span>
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
