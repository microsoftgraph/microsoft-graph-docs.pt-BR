---
title: Criar certificateBasedAuthConfiguration
description: Use esta API para criar um novo certificateBasedAuthConfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc1c4462c3c0ae63a46b4f78c7487a7ccbe364ca
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37632575"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="957fa-103">Criar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="957fa-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="957fa-104">Criar um novo objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="957fa-104">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="957fa-105">Só é possível criar uma única instância de um **certificateBasedAuthConfiguration** (a coleção só pode ter um membro).</span><span class="sxs-lookup"><span data-stu-id="957fa-105">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="957fa-106">Ele sempre tem uma ID fixa com um valor de ' 29728ade-6ae4-4ee9-9103-412912537da5 '.</span><span class="sxs-lookup"><span data-stu-id="957fa-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="957fa-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="957fa-107">Permissions</span></span>

<span data-ttu-id="957fa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="957fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="957fa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="957fa-110">Permission type</span></span>                        | <span data-ttu-id="957fa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="957fa-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="957fa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="957fa-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="957fa-113">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="957fa-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="957fa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="957fa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="957fa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="957fa-115">Not supported.</span></span> |
| <span data-ttu-id="957fa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="957fa-116">Application</span></span>    | <span data-ttu-id="957fa-117">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="957fa-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="957fa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="957fa-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="957fa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="957fa-119">Request headers</span></span>

| <span data-ttu-id="957fa-120">Nome</span><span class="sxs-lookup"><span data-stu-id="957fa-120">Name</span></span>          | <span data-ttu-id="957fa-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="957fa-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="957fa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="957fa-122">Authorization</span></span> | <span data-ttu-id="957fa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="957fa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="957fa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="957fa-125">Content-Type</span></span> | <span data-ttu-id="957fa-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="957fa-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="957fa-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="957fa-128">Request body</span></span>

<span data-ttu-id="957fa-129">As propriedades a seguir são necessárias para criar o objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="957fa-129">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="957fa-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="957fa-130">Property</span></span>     | <span data-ttu-id="957fa-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="957fa-131">Type</span></span>        | <span data-ttu-id="957fa-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="957fa-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="957fa-133">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="957fa-133">certificateAuthorities</span></span>| <span data-ttu-id="957fa-134">coleção [certificateAuthority](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="957fa-134">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="957fa-135">Coleção de autoridades de certificação que cria uma cadeia de certificado confiável.</span><span class="sxs-lookup"><span data-stu-id="957fa-135">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="957fa-136">Cada membro da coleção deve conter Propriedades de **certificado** e **isRootAuthority** .</span><span class="sxs-lookup"><span data-stu-id="957fa-136">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="957fa-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="957fa-137">Response</span></span>

<span data-ttu-id="957fa-138">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="957fa-138">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="957fa-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="957fa-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="957fa-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="957fa-140">Request</span></span>

<span data-ttu-id="957fa-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="957fa-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="957fa-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="957fa-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}-->

```http
POST https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="957fa-143">C#</span><span class="sxs-lookup"><span data-stu-id="957fa-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="957fa-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="957fa-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="957fa-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="957fa-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="957fa-146">Java</span><span class="sxs-lookup"><span data-stu-id="957fa-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="957fa-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="957fa-147">Response</span></span>

<span data-ttu-id="957fa-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="957fa-148">The following is an example of the response.</span></span>

> <span data-ttu-id="957fa-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="957fa-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
