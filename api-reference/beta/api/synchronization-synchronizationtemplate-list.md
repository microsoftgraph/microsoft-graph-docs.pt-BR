---
title: Listar modelos de sincronização existentes
description: Lista os modelos de sincronização associados a um determinado aplicativo ou entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fa6cff80d76b12092801d9deea3d5c2d209c21d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452908"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="1d7ff-103">Listar modelos de sincronização existentes</span><span class="sxs-lookup"><span data-stu-id="1d7ff-103">List existing synchronization templates</span></span>

<span data-ttu-id="1d7ff-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1d7ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d7ff-105">Lista os modelos de sincronização associados a um determinado aplicativo ou entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-105">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d7ff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d7ff-106">Permissions</span></span>
<span data-ttu-id="1d7ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d7ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d7ff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d7ff-109">Permission type</span></span>                        | <span data-ttu-id="1d7ff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d7ff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d7ff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d7ff-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="1d7ff-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7ff-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="1d7ff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d7ff-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="1d7ff-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-114">Not supported.</span></span>|
|<span data-ttu-id="1d7ff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d7ff-115">Application</span></span>                            |<span data-ttu-id="1d7ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="1d7ff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d7ff-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="1d7ff-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d7ff-118">Request headers</span></span>

| <span data-ttu-id="1d7ff-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1d7ff-119">Name</span></span>           | <span data-ttu-id="1d7ff-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d7ff-120">Type</span></span>    | <span data-ttu-id="1d7ff-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d7ff-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="1d7ff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d7ff-122">Authorization</span></span>  | <span data-ttu-id="1d7ff-123">string</span><span class="sxs-lookup"><span data-stu-id="1d7ff-123">string</span></span>  | <span data-ttu-id="1d7ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d7ff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d7ff-126">Request body</span></span>

<span data-ttu-id="1d7ff-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="1d7ff-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d7ff-128">Response</span></span>

<span data-ttu-id="1d7ff-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e acollection dos objetos [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-129">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="1d7ff-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d7ff-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1d7ff-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d7ff-131">Request</span></span>
<span data-ttu-id="1d7ff-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d7ff-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d7ff-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```
# <a name="c"></a>[<span data-ttu-id="1d7ff-134">C#</span><span class="sxs-lookup"><span data-stu-id="1d7ff-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d7ff-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d7ff-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d7ff-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d7ff-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1d7ff-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d7ff-137">Response</span></span>
<span data-ttu-id="1d7ff-138">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-138">The following is an example of a response.</span></span>
><span data-ttu-id="1d7ff-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1d7ff-140">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d7ff-140">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "Slack",
            "factoryTag": "CustomSCIM",
            "schema": {
                    "directories": [],
                    "synchronizationRules": []
                    }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
