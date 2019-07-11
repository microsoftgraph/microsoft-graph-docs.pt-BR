---
title: Listar modelos de sincronização existentes
description: Lista os modelos de sincronização associados a um determinado aplicativo ou entidade de serviço.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4542352e4edf704ff8c3c8575d8a999b113582d0
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620420"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="717bf-103">Listar modelos de sincronização existentes</span><span class="sxs-lookup"><span data-stu-id="717bf-103">List existing synchronization templates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="717bf-104">Lista os modelos de sincronização associados a um determinado aplicativo ou entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="717bf-104">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="717bf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="717bf-105">Permissions</span></span>
<span data-ttu-id="717bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="717bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="717bf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="717bf-108">Permission type</span></span>                        | <span data-ttu-id="717bf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="717bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="717bf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="717bf-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="717bf-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="717bf-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="717bf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="717bf-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="717bf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="717bf-113">Not supported.</span></span>|
|<span data-ttu-id="717bf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="717bf-114">Application</span></span>                            |<span data-ttu-id="717bf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="717bf-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="717bf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="717bf-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="717bf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="717bf-117">Request headers</span></span>

| <span data-ttu-id="717bf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="717bf-118">Name</span></span>           | <span data-ttu-id="717bf-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="717bf-119">Type</span></span>    | <span data-ttu-id="717bf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="717bf-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="717bf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="717bf-121">Authorization</span></span>  | <span data-ttu-id="717bf-122">string</span><span class="sxs-lookup"><span data-stu-id="717bf-122">string</span></span>  | <span data-ttu-id="717bf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="717bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="717bf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="717bf-125">Request body</span></span>

<span data-ttu-id="717bf-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="717bf-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="717bf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="717bf-127">Response</span></span>

<span data-ttu-id="717bf-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e acollection dos objetos [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="717bf-128">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="717bf-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="717bf-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="717bf-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="717bf-130">Request</span></span>
<span data-ttu-id="717bf-131">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="717bf-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="717bf-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="717bf-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="717bf-133">C#</span><span class="sxs-lookup"><span data-stu-id="717bf-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="717bf-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="717bf-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="717bf-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="717bf-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="717bf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="717bf-136">Response</span></span>
<span data-ttu-id="717bf-137">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="717bf-137">The following is an example of a response.</span></span>
><span data-ttu-id="717bf-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="717bf-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="717bf-139">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="717bf-139">All the properties will be returned in an actual call.</span></span>
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
