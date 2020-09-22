---
title: Atualizar externalConnection
description: Atualizar as propriedades de um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b2cb23f1f3acb56d8a9c11542b15717f45c217a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006818"
---
# <a name="update-connection"></a><span data-ttu-id="f11d7-103">Atualizar conexão</span><span class="sxs-lookup"><span data-stu-id="f11d7-103">Update connection</span></span>

<span data-ttu-id="f11d7-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f11d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f11d7-105">Atualizar as propriedades de um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f11d7-105">Update the properties of an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="f11d7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f11d7-106">Permissions</span></span>

<span data-ttu-id="f11d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f11d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f11d7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f11d7-109">Permission type</span></span>                        | <span data-ttu-id="f11d7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f11d7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f11d7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f11d7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f11d7-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f11d7-112">Not supported.</span></span> |
| <span data-ttu-id="f11d7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f11d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f11d7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f11d7-114">Not supported.</span></span> |
| <span data-ttu-id="f11d7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f11d7-115">Application</span></span>                            | <span data-ttu-id="f11d7-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f11d7-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f11d7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f11d7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f11d7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f11d7-118">Request headers</span></span>

| <span data-ttu-id="f11d7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f11d7-119">Name</span></span>          | <span data-ttu-id="f11d7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f11d7-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="f11d7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f11d7-121">Authorization</span></span> | <span data-ttu-id="f11d7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f11d7-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f11d7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f11d7-124">Content-Type</span></span>  | <span data-ttu-id="f11d7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f11d7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f11d7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f11d7-127">Request body</span></span>

<span data-ttu-id="f11d7-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f11d7-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f11d7-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f11d7-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f11d7-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f11d7-130">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="f11d7-131">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="f11d7-131">The following properties can be updated.</span></span>

| <span data-ttu-id="f11d7-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f11d7-132">Property</span></span>      | <span data-ttu-id="f11d7-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f11d7-133">Type</span></span>                                           | <span data-ttu-id="f11d7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f11d7-134">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="f11d7-135">configuration</span><span class="sxs-lookup"><span data-stu-id="f11d7-135">configuration</span></span> | [<span data-ttu-id="f11d7-136">configuration</span><span class="sxs-lookup"><span data-stu-id="f11d7-136">configuration</span></span>](../resources/configuration.md) | <span data-ttu-id="f11d7-137">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar o conteúdo na conexão.</span><span class="sxs-lookup"><span data-stu-id="f11d7-137">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="f11d7-138">description</span><span class="sxs-lookup"><span data-stu-id="f11d7-138">description</span></span>   | <span data-ttu-id="f11d7-139">String</span><span class="sxs-lookup"><span data-stu-id="f11d7-139">String</span></span>                                         | <span data-ttu-id="f11d7-140">Descrição da conexão exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f11d7-140">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="f11d7-141">nome</span><span class="sxs-lookup"><span data-stu-id="f11d7-141">name</span></span>          | <span data-ttu-id="f11d7-142">String</span><span class="sxs-lookup"><span data-stu-id="f11d7-142">String</span></span>                                         | <span data-ttu-id="f11d7-143">O nome de exibição da conexão a ser exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f11d7-143">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="f11d7-144">Comprimento máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="f11d7-144">Maximum length of 128 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="f11d7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f11d7-145">Response</span></span>

<span data-ttu-id="f11d7-146">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f11d7-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f11d7-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f11d7-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f11d7-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f11d7-148">Request</span></span>

<span data-ttu-id="f11d7-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f11d7-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f11d7-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="f11d7-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connection"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr
Content-type: application/json

{
  "name": "Contoso HR Service Tickets",
  "description": "Connection to index HR service tickets"
}
```
# <a name="c"></a>[<span data-ttu-id="f11d7-151">C#</span><span class="sxs-lookup"><span data-stu-id="f11d7-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f11d7-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f11d7-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f11d7-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f11d7-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="f11d7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f11d7-154">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="f11d7-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f11d7-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


