---
title: Atualizar externalConnection
description: Atualizar as propriedades de um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7e2b6418c9dcbdc89fc7701302ddf28a780cb6d0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954649"
---
# <a name="update-connection"></a><span data-ttu-id="1a2a3-103">Atualizar conexão</span><span class="sxs-lookup"><span data-stu-id="1a2a3-103">Update connection</span></span>

<span data-ttu-id="1a2a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a2a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a2a3-105">Atualizar as propriedades de um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="1a2a3-105">Update the properties of an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="1a2a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a2a3-106">Permissions</span></span>

<span data-ttu-id="1a2a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a2a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a2a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a2a3-109">Permission type</span></span>                        | <span data-ttu-id="1a2a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a2a3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a2a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a2a3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a2a3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-112">Not supported.</span></span> |
| <span data-ttu-id="1a2a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a2a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a2a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-114">Not supported.</span></span> |
| <span data-ttu-id="1a2a3-115">Application</span><span class="sxs-lookup"><span data-stu-id="1a2a3-115">Application</span></span>                            | <span data-ttu-id="1a2a3-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a2a3-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a2a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a2a3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1a2a3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a2a3-118">Request headers</span></span>

| <span data-ttu-id="1a2a3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1a2a3-119">Name</span></span>          | <span data-ttu-id="1a2a3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a2a3-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="1a2a3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a2a3-121">Authorization</span></span> | <span data-ttu-id="1a2a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1a2a3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a2a3-124">Content-Type</span></span>  | <span data-ttu-id="1a2a3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a2a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a2a3-127">Request body</span></span>

<span data-ttu-id="1a2a3-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1a2a3-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1a2a3-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-130">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="1a2a3-131">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-131">The following properties can be updated.</span></span>

| <span data-ttu-id="1a2a3-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a2a3-132">Property</span></span>      | <span data-ttu-id="1a2a3-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a2a3-133">Type</span></span>                                           | <span data-ttu-id="1a2a3-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a2a3-134">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="1a2a3-135">configuração</span><span class="sxs-lookup"><span data-stu-id="1a2a3-135">configuration</span></span> | [<span data-ttu-id="1a2a3-136">configuration</span><span class="sxs-lookup"><span data-stu-id="1a2a3-136">configuration</span></span>](../resources/configuration.md) | <span data-ttu-id="1a2a3-137">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar o conteúdo na conexão.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-137">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="1a2a3-138">description</span><span class="sxs-lookup"><span data-stu-id="1a2a3-138">description</span></span>   | <span data-ttu-id="1a2a3-139">String</span><span class="sxs-lookup"><span data-stu-id="1a2a3-139">String</span></span>                                         | <span data-ttu-id="1a2a3-140">Descrição da conexão exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-140">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="1a2a3-141">nome</span><span class="sxs-lookup"><span data-stu-id="1a2a3-141">name</span></span>          | <span data-ttu-id="1a2a3-142">String</span><span class="sxs-lookup"><span data-stu-id="1a2a3-142">String</span></span>                                         | <span data-ttu-id="1a2a3-143">O nome de exibição da conexão a ser exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-143">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="1a2a3-144">Comprimento máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-144">Maximum length of 128 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="1a2a3-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a2a3-145">Response</span></span>

<span data-ttu-id="1a2a3-146">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1a2a3-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1a2a3-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a2a3-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a2a3-148">Request</span></span>

<span data-ttu-id="1a2a3-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a2a3-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a2a3-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1a2a3-151">C#</span><span class="sxs-lookup"><span data-stu-id="1a2a3-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a2a3-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a2a3-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a2a3-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a2a3-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a2a3-154">Java</span><span class="sxs-lookup"><span data-stu-id="1a2a3-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="1a2a3-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a2a3-155">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="1a2a3-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a2a3-156">The following is an example of the response.</span></span>

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


