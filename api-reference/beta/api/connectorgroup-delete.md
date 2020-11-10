---
title: Excluir connectorGroup
description: Excluir um conector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 389f7ba94bce852328ed415b5dfa1c9476daba01
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957419"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="3a620-103">Excluir connectorGroup</span><span class="sxs-lookup"><span data-stu-id="3a620-103">Delete connectorGroup</span></span>

<span data-ttu-id="3a620-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a620-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a620-105">Excluir um [conector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="3a620-105">Delete a [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="3a620-106">Todos os [conectores](../resources/connector.md) e aplicativos devem ser removidos do grupo de conectores para que um grupo de conectores possa ser excluído.</span><span class="sxs-lookup"><span data-stu-id="3a620-106">All [connectors](../resources/connector.md) and applications must be removed from the connector group before a connector group can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a620-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a620-107">Permissions</span></span>
<span data-ttu-id="3a620-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a620-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3a620-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a620-110">Permission type</span></span>      | <span data-ttu-id="3a620-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a620-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a620-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a620-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a620-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a620-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3a620-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a620-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a620-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a620-115">Not supported.</span></span>    |
|<span data-ttu-id="3a620-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a620-116">Application</span></span> | <span data-ttu-id="3a620-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a620-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3a620-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a620-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3a620-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a620-119">Request headers</span></span>
| <span data-ttu-id="3a620-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3a620-120">Name</span></span>       | <span data-ttu-id="3a620-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a620-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3a620-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a620-122">Authorization</span></span>  | <span data-ttu-id="3a620-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="3a620-123">Bearer.</span></span> <span data-ttu-id="3a620-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="3a620-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a620-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a620-125">Request body</span></span>
<span data-ttu-id="3a620-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a620-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a620-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a620-127">Response</span></span>

<span data-ttu-id="3a620-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a620-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a620-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a620-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a620-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a620-131">Request</span></span>
<span data-ttu-id="3a620-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a620-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a620-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a620-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="3a620-134">C#</span><span class="sxs-lookup"><span data-stu-id="3a620-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a620-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a620-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a620-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a620-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a620-137">Java</span><span class="sxs-lookup"><span data-stu-id="3a620-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3a620-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a620-138">Response</span></span>
<span data-ttu-id="3a620-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a620-139">The following is an example of the response.</span></span> <span data-ttu-id="3a620-140">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3a620-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3a620-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a620-141">All of the properties will be returned from an actual call.</span></span>
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


