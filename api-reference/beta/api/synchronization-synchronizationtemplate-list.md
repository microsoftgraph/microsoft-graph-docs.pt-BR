---
title: Listar modelos de sincronização existentes
description: Lista os modelos de sincronização associados a um determinado aplicativo ou entidade de serviço.
localization_priority: Normal
ms.openlocfilehash: 01ddd6f02bfab06be6e2111e6bd0169492449b9d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271229"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="2b141-103">Listar modelos de sincronização existentes</span><span class="sxs-lookup"><span data-stu-id="2b141-103">List existing synchronization templates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b141-104">Lista os modelos de sincronização associados a um determinado aplicativo ou entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="2b141-104">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b141-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b141-105">Permissions</span></span>
<span data-ttu-id="2b141-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b141-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b141-108">Permission type</span></span>                        | <span data-ttu-id="2b141-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b141-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b141-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b141-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="2b141-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b141-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="2b141-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b141-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="2b141-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b141-113">Not supported.</span></span>|
|<span data-ttu-id="2b141-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b141-114">Application</span></span>                            |<span data-ttu-id="2b141-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b141-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="2b141-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b141-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="2b141-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b141-117">Request headers</span></span>

| <span data-ttu-id="2b141-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2b141-118">Name</span></span>           | <span data-ttu-id="2b141-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b141-119">Type</span></span>    | <span data-ttu-id="2b141-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b141-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="2b141-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b141-121">Authorization</span></span>  | <span data-ttu-id="2b141-122">string</span><span class="sxs-lookup"><span data-stu-id="2b141-122">string</span></span>  | <span data-ttu-id="2b141-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b141-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b141-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b141-125">Request body</span></span>

<span data-ttu-id="2b141-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b141-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="2b141-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b141-127">Response</span></span>

<span data-ttu-id="2b141-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e acollection dos objetos [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b141-128">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="2b141-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b141-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2b141-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b141-130">Request</span></span>
<span data-ttu-id="2b141-131">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b141-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```

##### <a name="response"></a><span data-ttu-id="2b141-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b141-132">Response</span></span>
<span data-ttu-id="2b141-133">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="2b141-133">The following is an example of a response.</span></span>
><span data-ttu-id="2b141-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2b141-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2b141-135">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b141-135">All the properties will be returned in an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2b141-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2b141-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2b141-137">C#</span><span class="sxs-lookup"><span data-stu-id="2b141-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationtemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b141-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="2b141-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationtemplate-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2b141-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2b141-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_synchronizationtemplate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
