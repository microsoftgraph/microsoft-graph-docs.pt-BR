---
title: Excluir connectorGroup
description: Excluir um conector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5f014aee2b518066fad0c8e8e4768d98eba21518
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982308"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="eee48-103">Excluir connectorGroup</span><span class="sxs-lookup"><span data-stu-id="eee48-103">Delete connectorGroup</span></span>

<span data-ttu-id="eee48-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eee48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eee48-105">Excluir um [conector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="eee48-105">Delete a [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="eee48-106">Todos os [conectores](../resources/connector.md) e aplicativos devem ser removidos do grupo de conectores para que um grupo de conectores possa ser excluído.</span><span class="sxs-lookup"><span data-stu-id="eee48-106">All [connectors](../resources/connector.md) and applications must be removed from the connector group before a connector group can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="eee48-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eee48-107">Permissions</span></span>
<span data-ttu-id="eee48-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eee48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eee48-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eee48-110">Permission type</span></span>      | <span data-ttu-id="eee48-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eee48-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eee48-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eee48-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eee48-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eee48-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eee48-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eee48-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eee48-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eee48-115">Not supported.</span></span>    |
|<span data-ttu-id="eee48-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eee48-116">Application</span></span> | <span data-ttu-id="eee48-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eee48-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="eee48-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eee48-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eee48-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eee48-119">Request headers</span></span>
| <span data-ttu-id="eee48-120">Nome</span><span class="sxs-lookup"><span data-stu-id="eee48-120">Name</span></span>       | <span data-ttu-id="eee48-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eee48-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eee48-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eee48-122">Authorization</span></span>  | <span data-ttu-id="eee48-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="eee48-123">Bearer.</span></span> <span data-ttu-id="eee48-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="eee48-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="eee48-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eee48-125">Request body</span></span>
<span data-ttu-id="eee48-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eee48-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eee48-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="eee48-127">Response</span></span>

<span data-ttu-id="eee48-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eee48-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eee48-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eee48-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eee48-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eee48-131">Request</span></span>
<span data-ttu-id="eee48-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eee48-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eee48-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="eee48-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="eee48-134">C#</span><span class="sxs-lookup"><span data-stu-id="eee48-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eee48-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eee48-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eee48-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eee48-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eee48-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="eee48-137">Response</span></span>
<span data-ttu-id="eee48-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eee48-138">The following is an example of the response.</span></span> <span data-ttu-id="eee48-139">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="eee48-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="eee48-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eee48-140">All of the properties will be returned from an actual call.</span></span>
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


