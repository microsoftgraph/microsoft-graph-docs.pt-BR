---
title: Criar publishedResource
description: Criar um novo objeto **publishedResource** .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5385959f1018d53614b2e5aee42d9293cf9108be
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973343"
---
# <a name="create-publishedresource"></a><span data-ttu-id="11cd9-103">Criar publishedResource</span><span class="sxs-lookup"><span data-stu-id="11cd9-103">Create publishedResource</span></span>

<span data-ttu-id="11cd9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11cd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11cd9-105">Criar um novo objeto [publishedResource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="11cd9-105">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="11cd9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="11cd9-106">Permissions</span></span>

<span data-ttu-id="11cd9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11cd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11cd9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11cd9-109">Permission type</span></span>                        | <span data-ttu-id="11cd9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11cd9-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="11cd9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11cd9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="11cd9-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11cd9-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="11cd9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11cd9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11cd9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11cd9-114">Not supported.</span></span> |
| <span data-ttu-id="11cd9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11cd9-115">Application</span></span>                            | <span data-ttu-id="11cd9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11cd9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11cd9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11cd9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="11cd9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11cd9-118">Request headers</span></span>

| <span data-ttu-id="11cd9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="11cd9-119">Name</span></span>      |<span data-ttu-id="11cd9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="11cd9-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="11cd9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="11cd9-121">Authorization</span></span> | <span data-ttu-id="11cd9-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="11cd9-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="11cd9-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11cd9-123">Request body</span></span>

<span data-ttu-id="11cd9-124">No corpo da solicitação, forneça uma representação JSON de um objeto [publishedResource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="11cd9-124">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="11cd9-125">Forneça os valores para as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="11cd9-125">Supply the values for the following properties.</span></span>

| <span data-ttu-id="11cd9-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11cd9-126">Property</span></span>     | <span data-ttu-id="11cd9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="11cd9-127">Type</span></span>        | <span data-ttu-id="11cd9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="11cd9-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="11cd9-129">displayName</span><span class="sxs-lookup"><span data-stu-id="11cd9-129">displayName</span></span>|<span data-ttu-id="11cd9-130">String</span><span class="sxs-lookup"><span data-stu-id="11cd9-130">String</span></span>|<span data-ttu-id="11cd9-131">Nome para exibição do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="11cd9-131">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="11cd9-132">resourceName</span><span class="sxs-lookup"><span data-stu-id="11cd9-132">resourceName</span></span>|<span data-ttu-id="11cd9-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11cd9-133">String</span></span>|<span data-ttu-id="11cd9-134">Nome do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="11cd9-134">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="11cd9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="11cd9-135">Response</span></span>

<span data-ttu-id="11cd9-136">Se bem-sucedido, este método retorna um `201 Created` código de resposta e um objeto [publishedResource](../resources/publishedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11cd9-136">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11cd9-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11cd9-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11cd9-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11cd9-138">Request</span></span>

<span data-ttu-id="11cd9-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11cd9-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11cd9-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="11cd9-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_publishedresource_from_onpremisespublishingprofile"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources
Content-Type: application/json

{
    "displayName": "New provisioning",
    "resourceName": "domain1.contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="11cd9-141">C#</span><span class="sxs-lookup"><span data-stu-id="11cd9-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-publishedresource-from-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11cd9-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11cd9-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-publishedresource-from-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11cd9-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11cd9-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-publishedresource-from-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11cd9-144">Java</span><span class="sxs-lookup"><span data-stu-id="11cd9-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-publishedresource-from-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11cd9-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="11cd9-145">Response</span></span>

<span data-ttu-id="11cd9-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11cd9-146">The following is an example of the response.</span></span>

> <span data-ttu-id="11cd9-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11cd9-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 201 Created

{
    "id": "4655ed41-1619-4848-92bb-0576d3038682",
    "publishingType": "provisioning",
    "displayName": "New provisionin",
    "resourceName": "domain1.contoso.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


