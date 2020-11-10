---
title: Criar certificateBasedAuthConfiguration
description: Use esta API para criar um novo certificateBasedAuthConfiguration.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f424ec111fb7551232bdf102b8debcb9dc248394
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959357"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="c4b8d-103">Criar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="c4b8d-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="c4b8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4b8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4b8d-105">Criar um novo objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c4b8d-105">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="c4b8d-106">Só é possível criar uma única instância de um **certificateBasedAuthConfiguration** (a coleção só pode ter um membro).</span><span class="sxs-lookup"><span data-stu-id="c4b8d-106">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="c4b8d-107">Ele sempre tem uma ID fixa com um valor de ' 29728ade-6ae4-4ee9-9103-412912537da5 '.</span><span class="sxs-lookup"><span data-stu-id="c4b8d-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4b8d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4b8d-108">Permissions</span></span>

<span data-ttu-id="c4b8d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4b8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4b8d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4b8d-111">Permission type</span></span>                        | <span data-ttu-id="c4b8d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4b8d-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c4b8d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4b8d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4b8d-114">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4b8d-114">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="c4b8d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4b8d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4b8d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4b8d-116">Not supported.</span></span> |
| <span data-ttu-id="c4b8d-117">Application</span><span class="sxs-lookup"><span data-stu-id="c4b8d-117">Application</span></span>    | <span data-ttu-id="c4b8d-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4b8d-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4b8d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4b8d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="c4b8d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4b8d-120">Request headers</span></span>

| <span data-ttu-id="c4b8d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c4b8d-121">Name</span></span>          | <span data-ttu-id="c4b8d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4b8d-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c4b8d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4b8d-123">Authorization</span></span> | <span data-ttu-id="c4b8d-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c4b8d-124">Bearer {token}</span></span> |
| <span data-ttu-id="c4b8d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4b8d-125">Content-Type</span></span> | <span data-ttu-id="c4b8d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4b8d-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4b8d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4b8d-127">Request body</span></span>

<span data-ttu-id="c4b8d-128">As propriedades a seguir são necessárias para criar o objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c4b8d-128">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="c4b8d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4b8d-129">Property</span></span>     | <span data-ttu-id="c4b8d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4b8d-130">Type</span></span>        | <span data-ttu-id="c4b8d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4b8d-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c4b8d-132">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="c4b8d-132">certificateAuthorities</span></span>| <span data-ttu-id="c4b8d-133">coleção [certificateAuthority](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="c4b8d-133">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="c4b8d-134">Coleção de autoridades de certificação que cria uma cadeia de certificado confiável.</span><span class="sxs-lookup"><span data-stu-id="c4b8d-134">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="c4b8d-135">Cada membro da coleção deve conter Propriedades de **certificado** e **isRootAuthority** .</span><span class="sxs-lookup"><span data-stu-id="c4b8d-135">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="c4b8d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4b8d-136">Response</span></span>

<span data-ttu-id="c4b8d-137">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4b8d-137">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4b8d-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c4b8d-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4b8d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4b8d-139">Request</span></span>

<span data-ttu-id="c4b8d-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4b8d-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4b8d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4b8d-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}-->

```http
POST https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration
Content-type: application/json

{
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificate": "Binary"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="c4b8d-142">C#</span><span class="sxs-lookup"><span data-stu-id="c4b8d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4b8d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4b8d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4b8d-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4b8d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4b8d-145">Java</span><span class="sxs-lookup"><span data-stu-id="c4b8d-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c4b8d-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4b8d-146">Response</span></span>

<span data-ttu-id="c4b8d-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4b8d-147">The following is an example of the response.</span></span>

> <span data-ttu-id="c4b8d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4b8d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificate": "Binary",
      "issuer": "issuer-value",
      "issuerSki": "issuerSki-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


