---
title: Criar publishedResource
description: Crie um novo **objeto publishedResource.**
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 0cf0b586010b6d68a36f4d710bc24f0035ecafa7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055159"
---
# <a name="create-publishedresource"></a><span data-ttu-id="c3f8c-103">Criar publishedResource</span><span class="sxs-lookup"><span data-stu-id="c3f8c-103">Create publishedResource</span></span>

<span data-ttu-id="c3f8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3f8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3f8c-105">Crie um novo [objeto publishedResource.](../resources/publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="c3f8c-105">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3f8c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3f8c-106">Permissions</span></span>

<span data-ttu-id="c3f8c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3f8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c3f8c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3f8c-109">Permission type</span></span>                        | <span data-ttu-id="c3f8c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3f8c-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3f8c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3f8c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c3f8c-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3f8c-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="c3f8c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3f8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3f8c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3f8c-114">Not supported.</span></span> |
| <span data-ttu-id="c3f8c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3f8c-115">Application</span></span>                            | <span data-ttu-id="c3f8c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3f8c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3f8c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3f8c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="c3f8c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3f8c-118">Request headers</span></span>

| <span data-ttu-id="c3f8c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c3f8c-119">Name</span></span>      |<span data-ttu-id="c3f8c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3f8c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3f8c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3f8c-121">Authorization</span></span> | <span data-ttu-id="c3f8c-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c3f8c-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3f8c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3f8c-123">Request body</span></span>

<span data-ttu-id="c3f8c-124">No corpo da solicitação, fornece uma representação JSON de um [objeto publishedResource.](../resources/publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="c3f8c-124">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="c3f8c-125">Fornecer os valores para as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="c3f8c-125">Supply the values for the following properties.</span></span>

| <span data-ttu-id="c3f8c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3f8c-126">Property</span></span>     | <span data-ttu-id="c3f8c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3f8c-127">Type</span></span>        | <span data-ttu-id="c3f8c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3f8c-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c3f8c-129">displayName</span><span class="sxs-lookup"><span data-stu-id="c3f8c-129">displayName</span></span>|<span data-ttu-id="c3f8c-130">String</span><span class="sxs-lookup"><span data-stu-id="c3f8c-130">String</span></span>|<span data-ttu-id="c3f8c-131">Nome de exibição do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="c3f8c-131">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="c3f8c-132">resourceName</span><span class="sxs-lookup"><span data-stu-id="c3f8c-132">resourceName</span></span>|<span data-ttu-id="c3f8c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3f8c-133">String</span></span>|<span data-ttu-id="c3f8c-134">Nome do publishedResource.</span><span class="sxs-lookup"><span data-stu-id="c3f8c-134">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="c3f8c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3f8c-135">Response</span></span>

<span data-ttu-id="c3f8c-136">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [publishedResource](../resources/publishedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3f8c-136">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3f8c-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c3f8c-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3f8c-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3f8c-138">Request</span></span>

<span data-ttu-id="c3f8c-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3f8c-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c3f8c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3f8c-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c3f8c-141">C#</span><span class="sxs-lookup"><span data-stu-id="c3f8c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-publishedresource-from-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3f8c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3f8c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-publishedresource-from-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3f8c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3f8c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-publishedresource-from-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3f8c-144">Java</span><span class="sxs-lookup"><span data-stu-id="c3f8c-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-publishedresource-from-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c3f8c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3f8c-145">Response</span></span>

<span data-ttu-id="c3f8c-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c3f8c-146">The following is an example of the response.</span></span>

> <span data-ttu-id="c3f8c-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c3f8c-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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



