---
title: Atualizar synchronizationtemplate
description: Atualizar (substituir) o modelo de sincronização associado a um determinado aplicativo.
localization_priority: Normal
ms.openlocfilehash: 219a303b01198c3fb4ac4bb00e8a91564f8cf3b2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637924"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="24651-103">Atualizar synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="24651-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24651-104">Atualizar (substituir) o modelo de sincronização associado a um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="24651-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="24651-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="24651-105">Permissions</span></span>
<span data-ttu-id="24651-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24651-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24651-108">Permission type</span></span>                        | <span data-ttu-id="24651-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24651-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="24651-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24651-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="24651-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24651-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="24651-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24651-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="24651-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24651-113">Not supported.</span></span>|
|<span data-ttu-id="24651-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24651-114">Application</span></span>                            |<span data-ttu-id="24651-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24651-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="24651-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24651-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="24651-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24651-117">Request headers</span></span>

| <span data-ttu-id="24651-118">Nome</span><span class="sxs-lookup"><span data-stu-id="24651-118">Name</span></span>           | <span data-ttu-id="24651-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="24651-119">Type</span></span>    | <span data-ttu-id="24651-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="24651-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="24651-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="24651-121">Authorization</span></span>  | <span data-ttu-id="24651-122">string</span><span class="sxs-lookup"><span data-stu-id="24651-122">string</span></span>  | <span data-ttu-id="24651-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24651-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24651-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24651-125">Request body</span></span>

<span data-ttu-id="24651-126">No corpo da solicitação, forneça o [](../resources/synchronization-synchronizationtemplate.md) objeto synchronizationtemplate para substituir o modelo existente.</span><span class="sxs-lookup"><span data-stu-id="24651-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="24651-127">Certifique-se de que todas as propriedades sejam fornecidas.</span><span class="sxs-lookup"><span data-stu-id="24651-127">Make sure all properties are provided.</span></span> <span data-ttu-id="24651-128">As propriedades ausentes serão apagadas.</span><span class="sxs-lookup"><span data-stu-id="24651-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="24651-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="24651-129">Response</span></span>

<span data-ttu-id="24651-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24651-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="24651-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="24651-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="24651-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24651-133">Request</span></span>
<span data-ttu-id="24651-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="24651-134">The following is an example of a request.</span></span> 

><span data-ttu-id="24651-135">**Observação:** O objeto Request mostrado aqui é reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24651-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="24651-136">Incluir todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24651-136">Include all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="24651-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="24651-137">Response</span></span>
<span data-ttu-id="24651-138">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="24651-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="24651-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="24651-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="24651-140">Basic</span><span class="sxs-lookup"><span data-stu-id="24651-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_synchronizationtemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24651-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24651-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_synchronizationtemplate-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
