---
title: Criar certificateBasedAuthConfiguration
description: Use essa API para criar um novo certificateBasedAuthConfiguration.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d8b67543ca5a943bfe595c0fd17cd196ad68c82c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047564"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="8b8e7-103">Criar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b8e7-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="8b8e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b8e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b8e7-105">Crie um novo [objeto certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b8e7-105">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="8b8e7-106">Somente uma única instância de **um certificateBasedAuthConfiguration** pode ser criada (a coleção só pode ter um membro).</span><span class="sxs-lookup"><span data-stu-id="8b8e7-106">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="8b8e7-107">Ele sempre tem uma ID fixa com um valor '29728ade-6ae4-4ee9-9103-412912537da5'.</span><span class="sxs-lookup"><span data-stu-id="8b8e7-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b8e7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b8e7-108">Permissions</span></span>

<span data-ttu-id="8b8e7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b8e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b8e7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b8e7-111">Permission type</span></span>                        | <span data-ttu-id="8b8e7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b8e7-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8b8e7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b8e7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b8e7-114">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b8e7-114">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="8b8e7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b8e7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b8e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b8e7-116">Not supported.</span></span> |
| <span data-ttu-id="8b8e7-117">Application</span><span class="sxs-lookup"><span data-stu-id="8b8e7-117">Application</span></span>    | <span data-ttu-id="8b8e7-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b8e7-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b8e7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b8e7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="8b8e7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b8e7-120">Request headers</span></span>

| <span data-ttu-id="8b8e7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8b8e7-121">Name</span></span>          | <span data-ttu-id="8b8e7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b8e7-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8b8e7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b8e7-123">Authorization</span></span> | <span data-ttu-id="8b8e7-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8b8e7-124">Bearer {token}</span></span> |
| <span data-ttu-id="8b8e7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b8e7-125">Content-Type</span></span> | <span data-ttu-id="8b8e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b8e7-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b8e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b8e7-127">Request body</span></span>

<span data-ttu-id="8b8e7-128">As propriedades a seguir são necessárias para criar o [objeto certificateBasedAuthConfiguration.](../resources/certificatebasedauthconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b8e7-128">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="8b8e7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b8e7-129">Property</span></span>     | <span data-ttu-id="8b8e7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b8e7-130">Type</span></span>        | <span data-ttu-id="8b8e7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b8e7-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8b8e7-132">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="8b8e7-132">certificateAuthorities</span></span>| <span data-ttu-id="8b8e7-133">[Coleção certificateAuthority](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="8b8e7-133">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="8b8e7-134">Coleção de autoridades de certificados que cria uma cadeia de certificados confiável.</span><span class="sxs-lookup"><span data-stu-id="8b8e7-134">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="8b8e7-135">Cada membro da coleção deve conter **propriedades certificate** e **isRootAuthority.**</span><span class="sxs-lookup"><span data-stu-id="8b8e7-135">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="8b8e7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b8e7-136">Response</span></span>

<span data-ttu-id="8b8e7-137">Se tiver êxito, este método retornará o código de resposta e `201 Created` um novo [objeto certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b8e7-137">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b8e7-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8b8e7-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b8e7-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b8e7-139">Request</span></span>

<span data-ttu-id="8b8e7-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b8e7-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b8e7-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b8e7-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8b8e7-142">C#</span><span class="sxs-lookup"><span data-stu-id="8b8e7-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b8e7-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b8e7-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b8e7-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b8e7-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b8e7-145">Java</span><span class="sxs-lookup"><span data-stu-id="8b8e7-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8b8e7-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b8e7-146">Response</span></span>

<span data-ttu-id="8b8e7-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8b8e7-147">The following is an example of the response.</span></span>

> <span data-ttu-id="8b8e7-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b8e7-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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


