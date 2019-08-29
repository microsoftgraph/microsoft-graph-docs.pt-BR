---
title: Criar certificateBasedAuthConfiguration
description: Use esta API para criar um novo certificateBasedAuthConfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc78cd5a2de6a8ce1b44dd346c6c19ad8741736f
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667607"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="3b52e-103">Criar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="3b52e-103">Create certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b52e-104">Criar um novo objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3b52e-104">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="3b52e-105">Só é possível criar uma única instância de um **certificateBasedAuthConfiguration** (a coleção só pode ter um membro).</span><span class="sxs-lookup"><span data-stu-id="3b52e-105">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="3b52e-106">Ele sempre tem uma ID fixa com um valor de ' 29728ade-6ae4-4ee9-9103-412912537da5 '.</span><span class="sxs-lookup"><span data-stu-id="3b52e-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b52e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b52e-107">Permissions</span></span>

<span data-ttu-id="3b52e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b52e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3b52e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b52e-110">Permission type</span></span>                        | <span data-ttu-id="3b52e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b52e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3b52e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b52e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3b52e-113">Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3b52e-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="3b52e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b52e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b52e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b52e-115">Not supported.</span></span> |
| <span data-ttu-id="3b52e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b52e-116">Application</span></span>    | <span data-ttu-id="3b52e-117">Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3b52e-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b52e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b52e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="3b52e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b52e-119">Request headers</span></span>

| <span data-ttu-id="3b52e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3b52e-120">Name</span></span>          | <span data-ttu-id="3b52e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b52e-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3b52e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b52e-122">Authorization</span></span> | <span data-ttu-id="3b52e-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="3b52e-123">Bearer {token}</span></span> |
| <span data-ttu-id="3b52e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b52e-124">Content-Type</span></span> | <span data-ttu-id="3b52e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b52e-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b52e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b52e-126">Request body</span></span>

<span data-ttu-id="3b52e-127">As propriedades a seguir são necessárias para criar o objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3b52e-127">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="3b52e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b52e-128">Property</span></span>     | <span data-ttu-id="3b52e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b52e-129">Type</span></span>        | <span data-ttu-id="3b52e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b52e-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3b52e-131">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="3b52e-131">certificateAuthorities</span></span>| <span data-ttu-id="3b52e-132">coleção [certificateAuthority](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="3b52e-132">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="3b52e-133">Coleção de autoridades de certificação que cria uma cadeia de certificado confiável.</span><span class="sxs-lookup"><span data-stu-id="3b52e-133">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="3b52e-134">Cada membro da coleção deve conter Propriedades de **certificado** e **isRootAuthority** .</span><span class="sxs-lookup"><span data-stu-id="3b52e-134">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="3b52e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b52e-135">Response</span></span>

<span data-ttu-id="3b52e-136">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b52e-136">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3b52e-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3b52e-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3b52e-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b52e-138">Request</span></span>

<span data-ttu-id="3b52e-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b52e-139">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3b52e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b52e-140">Response</span></span>

<span data-ttu-id="3b52e-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b52e-141">The following is an example of the response.</span></span>

> <span data-ttu-id="3b52e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b52e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
