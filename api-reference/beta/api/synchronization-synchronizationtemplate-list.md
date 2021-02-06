---
title: Listar modelos de sincronização existentes
description: Listar os modelos de sincronização associados a um determinado aplicativo ou entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 7a012dd73b61667a020d53a6190114054d1dccd1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137262"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="7f9f6-103">Listar modelos de sincronização existentes</span><span class="sxs-lookup"><span data-stu-id="7f9f6-103">List existing synchronization templates</span></span>

<span data-ttu-id="7f9f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f9f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f9f6-105">Listar os modelos de sincronização associados a um determinado aplicativo ou entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="7f9f6-105">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f9f6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f9f6-106">Permissions</span></span>
<span data-ttu-id="7f9f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f9f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f9f6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f9f6-109">Permission type</span></span>                        | <span data-ttu-id="7f9f6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f9f6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f9f6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f9f6-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="7f9f6-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f9f6-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7f9f6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f9f6-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7f9f6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f9f6-114">Not supported.</span></span>|
|<span data-ttu-id="7f9f6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f9f6-115">Application</span></span>                            |<span data-ttu-id="7f9f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f9f6-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="7f9f6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f9f6-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="7f9f6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9f6-118">Request headers</span></span>

| <span data-ttu-id="7f9f6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7f9f6-119">Name</span></span>           | <span data-ttu-id="7f9f6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f9f6-120">Type</span></span>    | <span data-ttu-id="7f9f6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f9f6-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7f9f6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f9f6-122">Authorization</span></span>  | <span data-ttu-id="7f9f6-123">string</span><span class="sxs-lookup"><span data-stu-id="7f9f6-123">string</span></span>  | <span data-ttu-id="7f9f6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f9f6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f9f6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9f6-126">Request body</span></span>

<span data-ttu-id="7f9f6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f9f6-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="7f9f6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9f6-128">Response</span></span>

<span data-ttu-id="7f9f6-129">Se bem-sucedido, este método retorna um código de `200 OK` resposta e uma acolleção de objetos [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f9f6-129">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="7f9f6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f9f6-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7f9f6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9f6-131">Request</span></span>
<span data-ttu-id="7f9f6-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f9f6-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f9f6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f9f6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```
# <a name="c"></a>[<span data-ttu-id="7f9f6-134">C#</span><span class="sxs-lookup"><span data-stu-id="7f9f6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f9f6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f9f6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f9f6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f9f6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f9f6-137">Java</span><span class="sxs-lookup"><span data-stu-id="7f9f6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7f9f6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9f6-138">Response</span></span>
<span data-ttu-id="7f9f6-139">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="7f9f6-139">The following is an example of a response.</span></span>
><span data-ttu-id="7f9f6-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7f9f6-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7f9f6-141">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f9f6-141">All the properties will be returned in an actual call.</span></span>
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


