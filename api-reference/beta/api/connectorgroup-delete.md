---
title: Excluir connectorGroup
description: Exclua um connectorGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: d08c319f16e3f2329a0f944c1b2d313395052990
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047186"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="87262-103">Excluir connectorGroup</span><span class="sxs-lookup"><span data-stu-id="87262-103">Delete connectorGroup</span></span>

<span data-ttu-id="87262-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87262-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87262-105">Excluir um [connectorGroup](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="87262-105">Delete a [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="87262-106">Todos [os conectores](../resources/connector.md) e aplicativos devem ser removidos do grupo de conectores antes que um grupo de conectores possa ser excluído.</span><span class="sxs-lookup"><span data-stu-id="87262-106">All [connectors](../resources/connector.md) and applications must be removed from the connector group before a connector group can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="87262-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="87262-107">Permissions</span></span>
<span data-ttu-id="87262-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87262-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="87262-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87262-110">Permission type</span></span>      | <span data-ttu-id="87262-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87262-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87262-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87262-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87262-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="87262-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="87262-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87262-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87262-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87262-115">Not supported.</span></span>    |
|<span data-ttu-id="87262-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87262-116">Application</span></span> | <span data-ttu-id="87262-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87262-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="87262-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87262-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="87262-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87262-119">Request headers</span></span>
| <span data-ttu-id="87262-120">Nome</span><span class="sxs-lookup"><span data-stu-id="87262-120">Name</span></span>       | <span data-ttu-id="87262-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="87262-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="87262-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="87262-122">Authorization</span></span>  | <span data-ttu-id="87262-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="87262-123">Bearer.</span></span> <span data-ttu-id="87262-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="87262-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="87262-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87262-125">Request body</span></span>
<span data-ttu-id="87262-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87262-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87262-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="87262-127">Response</span></span>

<span data-ttu-id="87262-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87262-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87262-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87262-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87262-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87262-131">Request</span></span>
<span data-ttu-id="87262-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87262-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87262-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="87262-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="87262-134">C#</span><span class="sxs-lookup"><span data-stu-id="87262-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87262-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87262-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87262-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87262-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87262-137">Java</span><span class="sxs-lookup"><span data-stu-id="87262-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="87262-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="87262-138">Response</span></span>
<span data-ttu-id="87262-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87262-139">The following is an example of the response.</span></span> <span data-ttu-id="87262-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="87262-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



