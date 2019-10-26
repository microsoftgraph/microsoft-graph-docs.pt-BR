---
title: 'trustFrameworkKeySet: uploadPkcs12'
description: Carregar uma chave PKCS 12 Format (PFX) em um conjunto de chaves.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e0ca40056c2b7e5607afdb9ffb1ea2cb314c2bc8
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734498"
---
# <a name="trustframeworkkeyset-uploadpkcs12"></a><span data-ttu-id="f2504-103">trustFrameworkKeySet: uploadPkcs12</span><span class="sxs-lookup"><span data-stu-id="f2504-103">trustFrameworkKeySet: uploadPkcs12</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2504-104">Carregar uma chave do formato PKCS12 (PFX) para um [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="f2504-104">Upload a PKCS12 format key (PFX) to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="f2504-105">A entrada é um valor codificado de base 64 do conteúdo do certificado PFX.</span><span class="sxs-lookup"><span data-stu-id="f2504-105">The input is a base-64 encoded value of the Pfx certificate contents.</span></span> <span data-ttu-id="f2504-106">Este método retorna [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="f2504-106">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2504-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2504-107">Permissions</span></span>

<span data-ttu-id="f2504-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2504-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2504-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2504-110">Permission type</span></span>                        | <span data-ttu-id="f2504-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2504-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f2504-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2504-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2504-113">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f2504-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="f2504-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2504-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2504-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2504-115">Not supported.</span></span> |
| <span data-ttu-id="f2504-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2504-116">Application</span></span>                            | <span data-ttu-id="f2504-117">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f2504-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2504-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2504-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadPkcs12
```

## <a name="request-headers"></a><span data-ttu-id="f2504-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2504-119">Request headers</span></span>

| <span data-ttu-id="f2504-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f2504-120">Name</span></span>          | <span data-ttu-id="f2504-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2504-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f2504-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2504-122">Authorization</span></span> | <span data-ttu-id="f2504-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2504-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2504-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="f2504-125">Content-type</span></span>  | <span data-ttu-id="f2504-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2504-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2504-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2504-128">Request body</span></span>

<span data-ttu-id="f2504-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2504-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f2504-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f2504-130">Parameter</span></span>    | <span data-ttu-id="f2504-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2504-131">Type</span></span>        | <span data-ttu-id="f2504-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2504-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f2504-133">key</span><span class="sxs-lookup"><span data-stu-id="f2504-133">key</span></span>|<span data-ttu-id="f2504-134">String</span><span class="sxs-lookup"><span data-stu-id="f2504-134">String</span></span>|<span data-ttu-id="f2504-135">Este é o campo para enviar conteúdo de PFX.</span><span class="sxs-lookup"><span data-stu-id="f2504-135">This is the field for sending pfx content.</span></span> <span data-ttu-id="f2504-136">O valor deve ser uma versão de codificação de base 64 do conteúdo de certificado real.</span><span class="sxs-lookup"><span data-stu-id="f2504-136">The value should be a base-64 encoded version of the actual certificate content.</span></span>|
|<span data-ttu-id="f2504-137">password</span><span class="sxs-lookup"><span data-stu-id="f2504-137">password</span></span>|<span data-ttu-id="f2504-138">String</span><span class="sxs-lookup"><span data-stu-id="f2504-138">String</span></span>|<span data-ttu-id="f2504-139">Este é o campo para enviar a senha para o conteúdo de PFX.</span><span class="sxs-lookup"><span data-stu-id="f2504-139">This is the field for sending the password to PFX content.</span></span>|

## <a name="response"></a><span data-ttu-id="f2504-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2504-140">Response</span></span>

<span data-ttu-id="f2504-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2504-141">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2504-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f2504-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2504-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2504-143">Request</span></span>

<span data-ttu-id="f2504-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2504-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadpkcs12"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadPkcs12
Content-type: application/json

{
  "key": "Base64-encoded-pfx-content",
  "password": "password-value"
}
```

### <a name="response"></a><span data-ttu-id="f2504-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2504-145">Response</span></span>

<span data-ttu-id="f2504-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f2504-146">The following is an example of the response.</span></span>

> <span data-ttu-id="f2504-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2504-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadPkcs12",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
