---
title: 'trustFrameworkKeySet: uploadSecret'
description: Carregar um segredo em um conjunto de chaves.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0d5a093541f1cd3cc322a4a161a425f6bf673f6f
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734497"
---
# <a name="trustframeworkkeyset-uploadsecret"></a><span data-ttu-id="593fd-103">trustFrameworkKeySet: uploadSecret</span><span class="sxs-lookup"><span data-stu-id="593fd-103">trustFrameworkKeySet: uploadSecret</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="593fd-104">Carregar um segredo de texto sem formatação em um [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="593fd-104">Upload a plain text secret to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="593fd-105">Exemplos de segredos são segredos do aplicativo no Azure Active Directory, Google, Facebook ou qualquer outro provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="593fd-105">Examples of secrets are application secrets in Azure Active Directory, Google, Facebook, or any other identity provider.</span></span> <span data-ttu-id="593fd-106">o método his retorna [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="593fd-106">his method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="593fd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="593fd-107">Permissions</span></span>

<span data-ttu-id="593fd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="593fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="593fd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="593fd-110">Permission type</span></span>                        | <span data-ttu-id="593fd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="593fd-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="593fd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="593fd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="593fd-113">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="593fd-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="593fd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="593fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="593fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="593fd-115">Not supported.</span></span> |
| <span data-ttu-id="593fd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="593fd-116">Application</span></span>                            | <span data-ttu-id="593fd-117">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="593fd-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="593fd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="593fd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadSecret
```

## <a name="request-headers"></a><span data-ttu-id="593fd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="593fd-119">Request headers</span></span>

| <span data-ttu-id="593fd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="593fd-120">Name</span></span>          | <span data-ttu-id="593fd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="593fd-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="593fd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="593fd-122">Authorization</span></span> | <span data-ttu-id="593fd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="593fd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="593fd-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="593fd-125">Content-type</span></span>  | <span data-ttu-id="593fd-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="593fd-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="593fd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="593fd-128">Request body</span></span>

<span data-ttu-id="593fd-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="593fd-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="593fd-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="593fd-130">Parameter</span></span>    | <span data-ttu-id="593fd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="593fd-131">Type</span></span>        | <span data-ttu-id="593fd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="593fd-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="593fd-133">Use</span><span class="sxs-lookup"><span data-stu-id="593fd-133">use</span></span>|<span data-ttu-id="593fd-134">String</span><span class="sxs-lookup"><span data-stu-id="593fd-134">String</span></span>|<span data-ttu-id="593fd-135">Semelhante à propriedade **use** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="593fd-135">Similar to the **use** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="593fd-136">f</span><span class="sxs-lookup"><span data-stu-id="593fd-136">k</span></span>|<span data-ttu-id="593fd-137">String</span><span class="sxs-lookup"><span data-stu-id="593fd-137">String</span></span>|<span data-ttu-id="593fd-138">Semelhante à propriedade **k** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="593fd-138">Similar to the **k** property of **trustFrameworkKey**.</span></span> <span data-ttu-id="593fd-139">Este é o campo que é usado para enviar o segredo.</span><span class="sxs-lookup"><span data-stu-id="593fd-139">This is the field that is used to send the secret.</span></span>|
|<span data-ttu-id="593fd-140">nbf</span><span class="sxs-lookup"><span data-stu-id="593fd-140">nbf</span></span>|<span data-ttu-id="593fd-141">Int64</span><span class="sxs-lookup"><span data-stu-id="593fd-141">Int64</span></span>|<span data-ttu-id="593fd-142">Semelhante à propriedade **NBF** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="593fd-142">Similar to the **nbf** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="593fd-143">exp</span><span class="sxs-lookup"><span data-stu-id="593fd-143">exp</span></span>|<span data-ttu-id="593fd-144">Int64</span><span class="sxs-lookup"><span data-stu-id="593fd-144">Int64</span></span>|<span data-ttu-id="593fd-145">Semelhante à propriedade **exp** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="593fd-145">Similar to the **exp** property of **trustFrameworkKey**.</span></span>|

## <a name="response"></a><span data-ttu-id="593fd-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="593fd-146">Response</span></span>

<span data-ttu-id="593fd-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="593fd-147">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="593fd-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="593fd-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="593fd-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="593fd-149">Request</span></span>

<span data-ttu-id="593fd-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="593fd-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadsecret"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadSecret
Content-type: application/json

{
  "use": "use-value",
  "k": "application-secret-to-be-uploaded",
  "nbf": 1508969811,
  "exp": 1508973711
}
```

### <a name="response"></a><span data-ttu-id="593fd-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="593fd-151">Response</span></span>

<span data-ttu-id="593fd-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="593fd-152">The following is an example of the response.</span></span>

> <span data-ttu-id="593fd-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="593fd-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "use": "use-value",
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadSecret",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
