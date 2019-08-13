---
title: Criar publishedResource
description: Criar um novo objeto **publishedResource** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75e560ac96a5d8979cd5b0b7c9f76e9ba2d42b90
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309213"
---
# <a name="create-publishedresource"></a><span data-ttu-id="49ef9-103">Criar publishedResource</span><span class="sxs-lookup"><span data-stu-id="49ef9-103">Create publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49ef9-104">Criar um novo objeto [publishedResource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="49ef9-104">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="49ef9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="49ef9-105">Permissions</span></span>

<span data-ttu-id="49ef9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49ef9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49ef9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49ef9-108">Permission type</span></span>                        | <span data-ttu-id="49ef9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49ef9-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="49ef9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49ef9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="49ef9-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="49ef9-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="49ef9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49ef9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49ef9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49ef9-113">Not supported.</span></span> |
| <span data-ttu-id="49ef9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49ef9-114">Application</span></span>                            | <span data-ttu-id="49ef9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49ef9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49ef9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49ef9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="49ef9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49ef9-117">Request headers</span></span>

| <span data-ttu-id="49ef9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="49ef9-118">Name</span></span>      |<span data-ttu-id="49ef9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="49ef9-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49ef9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="49ef9-120">Authorization</span></span> | <span data-ttu-id="49ef9-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="49ef9-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="49ef9-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49ef9-122">Request body</span></span>

<span data-ttu-id="49ef9-123">No corpo da solicitação, forneça uma representação JSON de um objeto [publishedResource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="49ef9-123">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="49ef9-124">Forneça os valores para as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="49ef9-124">Supply the values for the following properties.</span></span>

| <span data-ttu-id="49ef9-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49ef9-125">Property</span></span>     | <span data-ttu-id="49ef9-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="49ef9-126">Type</span></span>        | <span data-ttu-id="49ef9-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="49ef9-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="49ef9-128">displayName</span><span class="sxs-lookup"><span data-stu-id="49ef9-128">displayName</span></span>|<span data-ttu-id="49ef9-129">String</span><span class="sxs-lookup"><span data-stu-id="49ef9-129">String</span></span>|<span data-ttu-id="49ef9-130">Nome para exibição do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="49ef9-130">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="49ef9-131">resourceName</span><span class="sxs-lookup"><span data-stu-id="49ef9-131">resourceName</span></span>|<span data-ttu-id="49ef9-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49ef9-132">String</span></span>|<span data-ttu-id="49ef9-133">Nome do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="49ef9-133">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="49ef9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="49ef9-134">Response</span></span>

<span data-ttu-id="49ef9-135">Se bem-sucedido, este método retorna um `201 Created` código de resposta e um objeto [publishedResource](../resources/publishedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49ef9-135">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49ef9-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="49ef9-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49ef9-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49ef9-137">Request</span></span>

<span data-ttu-id="49ef9-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="49ef9-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="49ef9-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="49ef9-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="49ef9-140">C#</span><span class="sxs-lookup"><span data-stu-id="49ef9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-publishedresource-from-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49ef9-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49ef9-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-publishedresource-from-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49ef9-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="49ef9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-publishedresource-from-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="49ef9-143">Java</span><span class="sxs-lookup"><span data-stu-id="49ef9-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-publishedresource-from-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="49ef9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="49ef9-144">Response</span></span>

<span data-ttu-id="49ef9-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="49ef9-145">The following is an example of the response.</span></span>

> <span data-ttu-id="49ef9-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49ef9-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
