---
title: Criar certificateBasedAuthConfiguration
description: Use essa API para criar um novo certificateBasedAuthConfiguration.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1f1c759cade945fb8dad05d82ae30c9044074e5f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051568"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="59c6e-103">Criar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="59c6e-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="59c6e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59c6e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="59c6e-105">Crie um novo [objeto certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59c6e-105">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="59c6e-106">Somente uma única instância de **um certificateBasedAuthConfiguration** pode ser criada (a coleção só pode ter um membro).</span><span class="sxs-lookup"><span data-stu-id="59c6e-106">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="59c6e-107">Ele sempre tem uma ID fixa com um valor '29728ade-6ae4-4ee9-9103-412912537da5'.</span><span class="sxs-lookup"><span data-stu-id="59c6e-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="59c6e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="59c6e-108">Permissions</span></span>

<span data-ttu-id="59c6e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59c6e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59c6e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59c6e-111">Permission type</span></span>                        | <span data-ttu-id="59c6e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59c6e-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="59c6e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59c6e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="59c6e-114">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59c6e-114">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="59c6e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59c6e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59c6e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59c6e-116">Not supported.</span></span> |
| <span data-ttu-id="59c6e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59c6e-117">Application</span></span>    | <span data-ttu-id="59c6e-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59c6e-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59c6e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59c6e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration/$ref
```

## <a name="request-headers"></a><span data-ttu-id="59c6e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59c6e-120">Request headers</span></span>

| <span data-ttu-id="59c6e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="59c6e-121">Name</span></span>          | <span data-ttu-id="59c6e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c6e-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="59c6e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="59c6e-123">Authorization</span></span> | <span data-ttu-id="59c6e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59c6e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59c6e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59c6e-126">Content-Type</span></span> | <span data-ttu-id="59c6e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59c6e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59c6e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59c6e-129">Request body</span></span>

<span data-ttu-id="59c6e-130">As propriedades a seguir são necessárias para criar o [objeto certificateBasedAuthConfiguration.](../resources/certificatebasedauthconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59c6e-130">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="59c6e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59c6e-131">Property</span></span>     | <span data-ttu-id="59c6e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="59c6e-132">Type</span></span>        | <span data-ttu-id="59c6e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c6e-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="59c6e-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="59c6e-134">certificateAuthorities</span></span>| <span data-ttu-id="59c6e-135">[Coleção certificateAuthority](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="59c6e-135">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="59c6e-136">Coleção de autoridades de certificados que cria uma cadeia de certificados confiável.</span><span class="sxs-lookup"><span data-stu-id="59c6e-136">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="59c6e-137">Cada membro da coleção deve conter **propriedades certificate** e **isRootAuthority.**</span><span class="sxs-lookup"><span data-stu-id="59c6e-137">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="59c6e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="59c6e-138">Response</span></span>

<span data-ttu-id="59c6e-139">Se tiver êxito, este método retornará o código de resposta e `201 Created` um novo [objeto certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59c6e-139">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59c6e-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="59c6e-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59c6e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59c6e-141">Request</span></span>

<span data-ttu-id="59c6e-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="59c6e-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59c6e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="59c6e-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="59c6e-144">C#</span><span class="sxs-lookup"><span data-stu-id="59c6e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59c6e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59c6e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59c6e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59c6e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59c6e-147">Java</span><span class="sxs-lookup"><span data-stu-id="59c6e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="59c6e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="59c6e-148">Response</span></span>

<span data-ttu-id="59c6e-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="59c6e-149">The following is an example of the response.</span></span>

> <span data-ttu-id="59c6e-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="59c6e-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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

