---
title: Criar certificateBasedAuthConfiguration
description: Use esta API para criar um novo certificateBasedAuthConfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a73dd112bbcf9570622d7ed29df063b176f2ac1f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538858"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="f593c-103">Criar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="f593c-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="f593c-104">Criar um novo objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f593c-104">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="f593c-105">Só é possível criar uma única instância de um **certificateBasedAuthConfiguration** (a coleção só pode ter um membro).</span><span class="sxs-lookup"><span data-stu-id="f593c-105">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="f593c-106">Ele sempre tem uma ID fixa com um valor de ' 29728ade-6ae4-4ee9-9103-412912537da5 '.</span><span class="sxs-lookup"><span data-stu-id="f593c-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="f593c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f593c-107">Permissions</span></span>

<span data-ttu-id="f593c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f593c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f593c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f593c-110">Permission type</span></span>                        | <span data-ttu-id="f593c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f593c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f593c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f593c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f593c-113">Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f593c-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="f593c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f593c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f593c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f593c-115">Not supported.</span></span> |
| <span data-ttu-id="f593c-116">Application</span><span class="sxs-lookup"><span data-stu-id="f593c-116">Application</span></span>    | <span data-ttu-id="f593c-117">Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f593c-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f593c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f593c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="f593c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f593c-119">Request headers</span></span>

| <span data-ttu-id="f593c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f593c-120">Name</span></span>          | <span data-ttu-id="f593c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f593c-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f593c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f593c-122">Authorization</span></span> | <span data-ttu-id="f593c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f593c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f593c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f593c-125">Content-Type</span></span> | <span data-ttu-id="f593c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f593c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f593c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f593c-128">Request body</span></span>

<span data-ttu-id="f593c-129">As propriedades a seguir são necessárias para criar o objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f593c-129">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="f593c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f593c-130">Property</span></span>     | <span data-ttu-id="f593c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f593c-131">Type</span></span>        | <span data-ttu-id="f593c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f593c-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f593c-133">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="f593c-133">certificateAuthorities</span></span>| <span data-ttu-id="f593c-134">coleção [certificateAuthority](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="f593c-134">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="f593c-135">Coleção de autoridades de certificação que cria uma cadeia de certificado confiável.</span><span class="sxs-lookup"><span data-stu-id="f593c-135">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="f593c-136">Cada membro da coleção deve conter Propriedades de **certificado** e **isRootAuthority** .</span><span class="sxs-lookup"><span data-stu-id="f593c-136">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="f593c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f593c-137">Response</span></span>

<span data-ttu-id="f593c-138">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f593c-138">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f593c-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f593c-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f593c-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f593c-140">Request</span></span>

<span data-ttu-id="f593c-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f593c-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f593c-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f593c-142">HTTP</span></span>](#tab/http)
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

---


### <a name="response"></a><span data-ttu-id="f593c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f593c-143">Response</span></span>

<span data-ttu-id="f593c-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f593c-144">The following is an example of the response.</span></span>

> <span data-ttu-id="f593c-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f593c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
