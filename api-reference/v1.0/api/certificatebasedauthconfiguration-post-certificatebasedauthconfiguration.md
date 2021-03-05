---
title: Criar certificateBasedAuthConfiguration
description: Use essa API para criar um novo certificateBasedAuthConfiguration.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fa9b96d3df3c03dd48f75142cfc58efc5d0b0cd8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434815"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="20f34-103">Criar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="20f34-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="20f34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20f34-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20f34-105">Crie um novo [objeto certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20f34-105">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="20f34-106">Somente uma única instância de **um certificateBasedAuthConfiguration** pode ser criada (a coleção só pode ter um membro).</span><span class="sxs-lookup"><span data-stu-id="20f34-106">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="20f34-107">Ele sempre tem uma ID fixa com um valor '29728ade-6ae4-4ee9-9103-412912537da5'.</span><span class="sxs-lookup"><span data-stu-id="20f34-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="20f34-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="20f34-108">Permissions</span></span>

<span data-ttu-id="20f34-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20f34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20f34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20f34-111">Permission type</span></span>                        | <span data-ttu-id="20f34-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20f34-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="20f34-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20f34-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="20f34-114">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20f34-114">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="20f34-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20f34-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20f34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20f34-116">Not supported.</span></span> |
| <span data-ttu-id="20f34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20f34-117">Application</span></span>    | <span data-ttu-id="20f34-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20f34-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20f34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20f34-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration/$ref
```

## <a name="request-headers"></a><span data-ttu-id="20f34-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20f34-120">Request headers</span></span>

| <span data-ttu-id="20f34-121">Nome</span><span class="sxs-lookup"><span data-stu-id="20f34-121">Name</span></span>          | <span data-ttu-id="20f34-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="20f34-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="20f34-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="20f34-123">Authorization</span></span> | <span data-ttu-id="20f34-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20f34-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20f34-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20f34-126">Content-Type</span></span> | <span data-ttu-id="20f34-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20f34-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20f34-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20f34-129">Request body</span></span>

<span data-ttu-id="20f34-130">As propriedades a seguir são necessárias para criar o [objeto certificateBasedAuthConfiguration.](../resources/certificatebasedauthconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="20f34-130">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="20f34-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20f34-131">Property</span></span>     | <span data-ttu-id="20f34-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="20f34-132">Type</span></span>        | <span data-ttu-id="20f34-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="20f34-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="20f34-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="20f34-134">certificateAuthorities</span></span>| <span data-ttu-id="20f34-135">[Coleção certificateAuthority](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="20f34-135">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="20f34-136">Coleção de autoridades de certificados que cria uma cadeia de certificados confiável.</span><span class="sxs-lookup"><span data-stu-id="20f34-136">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="20f34-137">Cada membro da coleção deve conter **propriedades certificate** e **isRootAuthority.**</span><span class="sxs-lookup"><span data-stu-id="20f34-137">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="20f34-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="20f34-138">Response</span></span>

<span data-ttu-id="20f34-139">Se tiver êxito, este método retornará o código de resposta e `201 Created` um novo [objeto certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20f34-139">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20f34-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20f34-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20f34-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20f34-141">Request</span></span>

<span data-ttu-id="20f34-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="20f34-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20f34-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="20f34-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}-->

```http
POST https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/$ref
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
# <a name="c"></a>[<span data-ttu-id="20f34-144">C#</span><span class="sxs-lookup"><span data-stu-id="20f34-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20f34-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20f34-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20f34-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20f34-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20f34-147">Java</span><span class="sxs-lookup"><span data-stu-id="20f34-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="20f34-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="20f34-148">Response</span></span>

<span data-ttu-id="20f34-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20f34-149">The following is an example of the response.</span></span>

> <span data-ttu-id="20f34-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20f34-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

