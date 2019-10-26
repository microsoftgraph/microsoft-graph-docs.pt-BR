---
title: 'trustFrameworkKeySet: uploadCertificate'
description: Carregar um certificado em um conjunto de chaves.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64e5354cb39f2c2ead70b32f46f06c64615dfca2
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734518"
---
# <a name="trustframeworkkeyset-uploadcertificate"></a><span data-ttu-id="dd552-103">trustFrameworkKeySet: uploadCertificate</span><span class="sxs-lookup"><span data-stu-id="dd552-103">trustFrameworkKeySet: uploadCertificate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd552-104">Carregar um certificado em um [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="dd552-104">Upload a certificate to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="dd552-105">A entrada é um valor codificado em base 64 do conteúdo do certificado.</span><span class="sxs-lookup"><span data-stu-id="dd552-105">The input is a base-64 encoded value of the certificate contents.</span></span> <span data-ttu-id="dd552-106">Este método retorna [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="dd552-106">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd552-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd552-107">Permissions</span></span>

<span data-ttu-id="dd552-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd552-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd552-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd552-110">Permission type</span></span>                        | <span data-ttu-id="dd552-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd552-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dd552-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd552-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd552-113">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dd552-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="dd552-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd552-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd552-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd552-115">Not supported.</span></span> |
| <span data-ttu-id="dd552-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd552-116">Application</span></span>                            | <span data-ttu-id="dd552-117">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dd552-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd552-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd552-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadCertificate
```

## <a name="request-headers"></a><span data-ttu-id="dd552-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd552-119">Request headers</span></span>

| <span data-ttu-id="dd552-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dd552-120">Name</span></span>          | <span data-ttu-id="dd552-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd552-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dd552-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd552-122">Authorization</span></span> | <span data-ttu-id="dd552-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd552-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="dd552-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="dd552-125">Content-type</span></span> | <span data-ttu-id="dd552-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd552-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd552-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd552-128">Request body</span></span>

<span data-ttu-id="dd552-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd552-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dd552-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dd552-130">Parameter</span></span>    | <span data-ttu-id="dd552-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd552-131">Type</span></span>        | <span data-ttu-id="dd552-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd552-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd552-133">key</span><span class="sxs-lookup"><span data-stu-id="dd552-133">key</span></span>|<span data-ttu-id="dd552-134">String</span><span class="sxs-lookup"><span data-stu-id="dd552-134">String</span></span>| <span data-ttu-id="dd552-135">Este é o campo para enviar conteúdo de certificado.</span><span class="sxs-lookup"><span data-stu-id="dd552-135">This is the field for sending certificate content.</span></span> <span data-ttu-id="dd552-136">O valor deve ser uma versão de codificação de base 64 do conteúdo de certificado real.</span><span class="sxs-lookup"><span data-stu-id="dd552-136">The value should be a base-64 encoded version of the actual certificate content.</span></span> |

## <a name="response"></a><span data-ttu-id="dd552-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd552-137">Response</span></span>

<span data-ttu-id="dd552-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd552-138">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd552-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dd552-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dd552-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd552-140">Request</span></span>

<span data-ttu-id="dd552-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd552-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadCertificate
Content-type: application/json

{
  "key": "key-value"
}
```

### <a name="response"></a><span data-ttu-id="dd552-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd552-142">Response</span></span>

<span data-ttu-id="dd552-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dd552-143">The following is an example of the response.</span></span>

> <span data-ttu-id="dd552-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd552-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "kid": "kid-value",
    "use": "sig",
    "kty": "oct",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
