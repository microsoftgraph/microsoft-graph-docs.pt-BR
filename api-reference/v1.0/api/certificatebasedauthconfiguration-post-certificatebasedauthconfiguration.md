---
title: Criar certificateBasedAuthConfiguration
description: Use esta API para criar um novo certificateBasedAuthConfiguration.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2a690be92dd0bef8291dd933846104e3c3dd0843
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905793"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="70ab1-103">Criar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="70ab1-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="70ab1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70ab1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70ab1-105">Criar um novo objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="70ab1-105">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="70ab1-106">Só é possível criar uma única instância de um **certificateBasedAuthConfiguration** (a coleção só pode ter um membro).</span><span class="sxs-lookup"><span data-stu-id="70ab1-106">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="70ab1-107">Ele sempre tem uma ID fixa com um valor de ' 29728ade-6ae4-4ee9-9103-412912537da5 '.</span><span class="sxs-lookup"><span data-stu-id="70ab1-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="70ab1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="70ab1-108">Permissions</span></span>

<span data-ttu-id="70ab1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70ab1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70ab1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70ab1-111">Permission type</span></span>                        | <span data-ttu-id="70ab1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70ab1-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="70ab1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70ab1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="70ab1-114">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70ab1-114">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="70ab1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70ab1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70ab1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70ab1-116">Not supported.</span></span> |
| <span data-ttu-id="70ab1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70ab1-117">Application</span></span>    | <span data-ttu-id="70ab1-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70ab1-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70ab1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70ab1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration/$ref
```

## <a name="request-headers"></a><span data-ttu-id="70ab1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70ab1-120">Request headers</span></span>

| <span data-ttu-id="70ab1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="70ab1-121">Name</span></span>          | <span data-ttu-id="70ab1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="70ab1-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="70ab1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="70ab1-123">Authorization</span></span> | <span data-ttu-id="70ab1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70ab1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70ab1-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70ab1-126">Content-Type</span></span> | <span data-ttu-id="70ab1-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70ab1-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70ab1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70ab1-129">Request body</span></span>

<span data-ttu-id="70ab1-130">As propriedades a seguir são necessárias para criar o objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="70ab1-130">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="70ab1-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70ab1-131">Property</span></span>     | <span data-ttu-id="70ab1-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="70ab1-132">Type</span></span>        | <span data-ttu-id="70ab1-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="70ab1-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="70ab1-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="70ab1-134">certificateAuthorities</span></span>| <span data-ttu-id="70ab1-135">coleção [certificateAuthority](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="70ab1-135">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="70ab1-136">Coleção de autoridades de certificação que cria uma cadeia de certificado confiável.</span><span class="sxs-lookup"><span data-stu-id="70ab1-136">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="70ab1-137">Cada membro da coleção deve conter Propriedades de **certificado** e **isRootAuthority** .</span><span class="sxs-lookup"><span data-stu-id="70ab1-137">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="70ab1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="70ab1-138">Response</span></span>

<span data-ttu-id="70ab1-139">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70ab1-139">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70ab1-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="70ab1-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="70ab1-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70ab1-141">Request</span></span>

<span data-ttu-id="70ab1-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="70ab1-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70ab1-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="70ab1-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="70ab1-144">C#</span><span class="sxs-lookup"><span data-stu-id="70ab1-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70ab1-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70ab1-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70ab1-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70ab1-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70ab1-147">Java</span><span class="sxs-lookup"><span data-stu-id="70ab1-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="70ab1-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="70ab1-148">Response</span></span>

<span data-ttu-id="70ab1-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="70ab1-149">The following is an example of the response.</span></span>

> <span data-ttu-id="70ab1-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70ab1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

