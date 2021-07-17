---
title: Atualizar externalConnection
description: Atualize as propriedades de um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 8b14abf1a010b8d28e80308077bcc5aa2f72eecf
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467550"
---
# <a name="update-connection"></a><span data-ttu-id="32f03-103">Atualizar conexão</span><span class="sxs-lookup"><span data-stu-id="32f03-103">Update connection</span></span>

<span data-ttu-id="32f03-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="32f03-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32f03-105">Atualize as propriedades de [um externalConnection](../resources/externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="32f03-105">Update the properties of an [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="32f03-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="32f03-106">Permissions</span></span>

<span data-ttu-id="32f03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32f03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32f03-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32f03-109">Permission type</span></span>                        | <span data-ttu-id="32f03-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32f03-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="32f03-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32f03-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="32f03-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f03-112">Not supported.</span></span> |
| <span data-ttu-id="32f03-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32f03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32f03-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f03-114">Not supported.</span></span> |
| <span data-ttu-id="32f03-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32f03-115">Application</span></span>                            | <span data-ttu-id="32f03-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="32f03-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="32f03-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32f03-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="32f03-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32f03-118">Request headers</span></span>

| <span data-ttu-id="32f03-119">Nome</span><span class="sxs-lookup"><span data-stu-id="32f03-119">Name</span></span>          | <span data-ttu-id="32f03-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="32f03-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="32f03-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="32f03-121">Authorization</span></span> | <span data-ttu-id="32f03-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32f03-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="32f03-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32f03-124">Content-Type</span></span>  | <span data-ttu-id="32f03-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32f03-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32f03-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32f03-127">Request body</span></span>

<span data-ttu-id="32f03-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="32f03-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="32f03-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="32f03-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="32f03-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="32f03-130">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="32f03-131">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="32f03-131">The following properties can be updated.</span></span>

| <span data-ttu-id="32f03-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32f03-132">Property</span></span>      | <span data-ttu-id="32f03-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="32f03-133">Type</span></span>                                           | <span data-ttu-id="32f03-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="32f03-134">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="32f03-135">configuração</span><span class="sxs-lookup"><span data-stu-id="32f03-135">configuration</span></span> | [<span data-ttu-id="32f03-136">microsoft.graph.externalConnectors.configuration</span><span class="sxs-lookup"><span data-stu-id="32f03-136">microsoft.graph.externalConnectors.configuration</span></span>](../resources/externalconnectors-configuration.md) | <span data-ttu-id="32f03-137">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar conteúdo na conexão.</span><span class="sxs-lookup"><span data-stu-id="32f03-137">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="32f03-138">description</span><span class="sxs-lookup"><span data-stu-id="32f03-138">description</span></span>   | <span data-ttu-id="32f03-139">String</span><span class="sxs-lookup"><span data-stu-id="32f03-139">String</span></span>                                         | <span data-ttu-id="32f03-140">Descrição da conexão exibida no Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="32f03-140">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="32f03-141">nome</span><span class="sxs-lookup"><span data-stu-id="32f03-141">name</span></span>          | <span data-ttu-id="32f03-142">String</span><span class="sxs-lookup"><span data-stu-id="32f03-142">String</span></span>                                         | <span data-ttu-id="32f03-143">O nome de exibição da conexão a ser exibida no Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="32f03-143">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="32f03-144">Comprimento máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="32f03-144">Maximum length of 128 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="32f03-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f03-145">Response</span></span>

<span data-ttu-id="32f03-146">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="32f03-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="32f03-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="32f03-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="32f03-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32f03-148">Request</span></span>

<span data-ttu-id="32f03-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="32f03-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="32f03-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="32f03-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connection",
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr
Content-type: application/json

{
  "name": "Contoso HR Service Tickets",
  "description": "Connection to index HR service tickets"
}
```
# <a name="c"></a>[<span data-ttu-id="32f03-151">C#</span><span class="sxs-lookup"><span data-stu-id="32f03-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32f03-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32f03-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32f03-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32f03-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32f03-154">Java</span><span class="sxs-lookup"><span data-stu-id="32f03-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="32f03-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f03-155">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="32f03-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="32f03-156">The following is an example of the response.</span></span>

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
