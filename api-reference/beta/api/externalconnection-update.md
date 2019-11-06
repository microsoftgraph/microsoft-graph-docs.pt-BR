---
title: Atualizar externalConnection
description: Atualizar as propriedades de um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4f9e521b8fb9c003a5850b80ac06088f10dff628
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994510"
---
# <a name="update-connection"></a><span data-ttu-id="6719b-103">Atualizar conexão</span><span class="sxs-lookup"><span data-stu-id="6719b-103">Update connection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6719b-104">Atualizar as propriedades de um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="6719b-104">Update the properties of an [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6719b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6719b-105">Permissions</span></span>

<span data-ttu-id="6719b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6719b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6719b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6719b-108">Permission type</span></span>                        | <span data-ttu-id="6719b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6719b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6719b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6719b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6719b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6719b-111">Not supported.</span></span> |
| <span data-ttu-id="6719b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6719b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6719b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6719b-113">Not supported.</span></span> |
| <span data-ttu-id="6719b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6719b-114">Application</span></span>                            | <span data-ttu-id="6719b-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6719b-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6719b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6719b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6719b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6719b-117">Request headers</span></span>

| <span data-ttu-id="6719b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6719b-118">Name</span></span>          | <span data-ttu-id="6719b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6719b-119">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="6719b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6719b-120">Authorization</span></span> | <span data-ttu-id="6719b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6719b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6719b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6719b-123">Content-Type</span></span>  | <span data-ttu-id="6719b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6719b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6719b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6719b-126">Request body</span></span>

<span data-ttu-id="6719b-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6719b-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6719b-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="6719b-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6719b-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6719b-129">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="6719b-130">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="6719b-130">The following properties can be updated.</span></span>

| <span data-ttu-id="6719b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6719b-131">Property</span></span>      | <span data-ttu-id="6719b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6719b-132">Type</span></span>                                           | <span data-ttu-id="6719b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6719b-133">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="6719b-134">Configuration</span><span class="sxs-lookup"><span data-stu-id="6719b-134">configuration</span></span> | [<span data-ttu-id="6719b-135">configuration</span><span class="sxs-lookup"><span data-stu-id="6719b-135">configuration</span></span>](../resources/configuration.md) | <span data-ttu-id="6719b-136">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar o conteúdo na conexão.</span><span class="sxs-lookup"><span data-stu-id="6719b-136">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="6719b-137">description</span><span class="sxs-lookup"><span data-stu-id="6719b-137">description</span></span>   | <span data-ttu-id="6719b-138">String</span><span class="sxs-lookup"><span data-stu-id="6719b-138">String</span></span>                                         | <span data-ttu-id="6719b-139">Descrição da conexão exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6719b-139">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="6719b-140">nome</span><span class="sxs-lookup"><span data-stu-id="6719b-140">name</span></span>          | <span data-ttu-id="6719b-141">String</span><span class="sxs-lookup"><span data-stu-id="6719b-141">String</span></span>                                         | <span data-ttu-id="6719b-142">O nome de exibição da conexão a ser exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6719b-142">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="6719b-143">Comprimento máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="6719b-143">Maximum length of 128 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="6719b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6719b-144">Response</span></span>

<span data-ttu-id="6719b-145">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6719b-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6719b-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6719b-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6719b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6719b-147">Request</span></span>

<span data-ttu-id="6719b-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6719b-148">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6719b-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="6719b-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6719b-150">C#</span><span class="sxs-lookup"><span data-stu-id="6719b-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6719b-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6719b-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6719b-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6719b-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="6719b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6719b-153">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="6719b-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6719b-154">The following is an example of the response.</span></span>

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
