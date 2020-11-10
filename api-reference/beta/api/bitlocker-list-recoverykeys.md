---
title: Listar recoveryKeys
description: Obtenha uma lista dos objetos bitlockerRecoveryKey e suas propriedades.
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 865e44cf6c8d696ed4da549bad05d50229e29601
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961299"
---
# <a name="list-recoverykeys"></a><span data-ttu-id="a8711-103">Listar recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="a8711-103">List recoveryKeys</span></span>
<span data-ttu-id="a8711-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8711-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8711-105">Obtenha uma lista dos objetos [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="a8711-105">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span> 

<span data-ttu-id="a8711-106">Essa operação não retorna a propriedade **Key** .</span><span class="sxs-lookup"><span data-stu-id="a8711-106">This operation does not return the **key** property.</span></span> <span data-ttu-id="a8711-107">Para obter informações sobre como ler a propriedade **Key** , consulte [Get bitlockerRecoveryKey](bitlockerrecoverykey-get.md).</span><span class="sxs-lookup"><span data-stu-id="a8711-107">For information about how to read the **key** property, see [Get bitlockerRecoveryKey](bitlockerrecoverykey-get.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8711-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8711-108">Permissions</span></span>
<span data-ttu-id="a8711-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8711-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8711-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8711-111">Permission type</span></span>|<span data-ttu-id="a8711-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a8711-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8711-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8711-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8711-114">BitLocker. ReadBasic. All, BitLocker. Read. All</span><span class="sxs-lookup"><span data-stu-id="a8711-114">BitLocker.ReadBasic.All, BitLocker.Read.All</span></span>|
|<span data-ttu-id="a8711-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8711-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8711-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8711-116">Not supported</span></span>|
|<span data-ttu-id="a8711-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8711-117">Application</span></span>|<span data-ttu-id="a8711-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8711-118">Not supported</span></span>|

><span data-ttu-id="a8711-119">**Observação** : para permissões delegadas para permitir que os aplicativos obtenham recursos do BitLockerRecoveryKey em nome do usuário conectado, o administrador do locatário deve ter atribuído ao usuário uma das seguintes funções ou o usuário deve ser o proprietário registrado do dispositivo para o qual a chave de recuperação do BitLocker foi originalmente com backup:</span><span class="sxs-lookup"><span data-stu-id="a8711-119">**Note** : For delegated permissions to allow apps to get BitLockerRecoveryKey resources on behalf of the signed-in user, the tenant administrator must have assigned the user one of the following roles, or the user must be the registered owner of the device that the BitLocker recovery key was originally backed up from:</span></span> 
* <span data-ttu-id="a8711-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="a8711-120">Global administrator</span></span>
* <span data-ttu-id="a8711-121">Administrador do dispositivo de nuvem</span><span class="sxs-lookup"><span data-stu-id="a8711-121">Cloud device administrator</span></span>
* <span data-ttu-id="a8711-122">Administrador da assistência técnica</span><span class="sxs-lookup"><span data-stu-id="a8711-122">Helpdesk administrator</span></span>
* <span data-ttu-id="a8711-123">Administrador de Serviço do Intune</span><span class="sxs-lookup"><span data-stu-id="a8711-123">Intune service administrator</span></span>
* <span data-ttu-id="a8711-124">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="a8711-124">Security administrator</span></span>
* <span data-ttu-id="a8711-125">Leitor de segurança</span><span class="sxs-lookup"><span data-stu-id="a8711-125">Security reader</span></span>
* <span data-ttu-id="a8711-126">Leitor global</span><span class="sxs-lookup"><span data-stu-id="a8711-126">Global reader</span></span>

## <a name="http-request"></a><span data-ttu-id="a8711-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8711-127">HTTP request</span></span>
<span data-ttu-id="a8711-128">Para obter uma lista de chaves do BitLocker dentro do locatário:</span><span class="sxs-lookup"><span data-stu-id="a8711-128">To get a list of BitLocker keys within the tenant:</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys
```

<span data-ttu-id="a8711-129">Para obter uma lista de chaves do BitLocker dentro do locatário filtrado pela **ID do dispositivo** :</span><span class="sxs-lookup"><span data-stu-id="a8711-129">To get a list of BitLocker keys within the tenant filtered by the **device id** :</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys?$filter=deviceId eq '{deviceId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8711-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a8711-130">Optional query parameters</span></span>
<span data-ttu-id="a8711-131">Este método dá suporte ao `$filter` parâmetro de consulta OData para filtrar os resultados pela **ID do dispositivo** em que o backup foi feito mais recentemente.</span><span class="sxs-lookup"><span data-stu-id="a8711-131">This method supports the `$filter` OData query parameter to filter results by the **device id** the key was most recently backed up to.</span></span> <span data-ttu-id="a8711-132">Para obter detalhes, consulte o [exemplo 2](#example-2).</span><span class="sxs-lookup"><span data-stu-id="a8711-132">For details, see [Example 2](#example-2).</span></span> <span data-ttu-id="a8711-133">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a8711-133">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="a8711-134">A resposta também pode conter um `odata.nextLink` , que você pode usar para percorrer o conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="a8711-134">The response might also contain an `odata.nextLink`, which you can use to page through the result set.</span></span> <span data-ttu-id="a8711-135">Para obter detalhes, consulte [paginação de dados do Microsoft Graph](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="a8711-135">For details, see [Paging Microsoft Graph data](/graph/paging).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8711-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8711-136">Request headers</span></span>
|<span data-ttu-id="a8711-137">Nome</span><span class="sxs-lookup"><span data-stu-id="a8711-137">Name</span></span>|<span data-ttu-id="a8711-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8711-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a8711-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8711-139">Authorization</span></span>|<span data-ttu-id="a8711-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8711-p105">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a8711-142">OCP-Client-Name</span><span class="sxs-lookup"><span data-stu-id="a8711-142">ocp-client-name</span></span>|<span data-ttu-id="a8711-143">Nome do aplicativo cliente executando a chamada à API.</span><span class="sxs-lookup"><span data-stu-id="a8711-143">Name of the client application performing the API call.</span></span> <span data-ttu-id="a8711-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8711-144">Required.</span></span>|
|<span data-ttu-id="a8711-145">OCP-Client-Version</span><span class="sxs-lookup"><span data-stu-id="a8711-145">ocp-client-version</span></span>|<span data-ttu-id="a8711-146">Versão do aplicativo cliente executando a chamada à API.</span><span class="sxs-lookup"><span data-stu-id="a8711-146">Version of the client application performing the API call.</span></span> <span data-ttu-id="a8711-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8711-147">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8711-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8711-148">Request body</span></span>
<span data-ttu-id="a8711-149">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8711-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8711-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8711-150">Response</span></span>

<span data-ttu-id="a8711-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8711-151">If successful, this method returns a `200 OK` response code and a collection of [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8711-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a8711-152">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="a8711-153">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="a8711-153">Example 1</span></span>
<span data-ttu-id="a8711-154">Recupere uma lista de chaves do BitLocker no locatário.</span><span class="sxs-lookup"><span data-stu-id="a8711-154">Retrieve a list of BitLocker keys in the tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="a8711-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8711-155">Request</span></span>
<span data-ttu-id="a8711-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8711-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a8711-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8711-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="a8711-158">C#</span><span class="sxs-lookup"><span data-stu-id="a8711-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8711-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8711-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8711-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8711-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8711-161">Java</span><span class="sxs-lookup"><span data-stu-id="a8711-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="a8711-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8711-162">Response</span></span>
<span data-ttu-id="a8711-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8711-163">The following is an example of the response.</span></span>

<span data-ttu-id="a8711-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a8711-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.bitlockerRecoveryKey)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "2ef04ef1-23b0-2e00-a3a5-ab345e567ab6"
    },
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "6a30ed7b-247b-4d26-86b5-2f405e55ea42",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```
### <a name="example-2"></a><span data-ttu-id="a8711-165">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="a8711-165">Example 2</span></span>
<span data-ttu-id="a8711-166">Recupere uma lista de chaves do BitLocker filtradas por **ID de dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="a8711-166">Retrieve a list of BitLocker keys filtered by **device id**.</span></span>

#### <a name="request"></a><span data-ttu-id="a8711-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8711-167">Request</span></span>
<span data-ttu-id="a8711-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8711-168">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a8711-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8711-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleIds": ["1ab40ab2-32a8-4b00-b6b5-ba724e407de9"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys?$filter=deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="a8711-170">C#</span><span class="sxs-lookup"><span data-stu-id="a8711-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8711-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8711-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8711-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8711-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8711-173">Java</span><span class="sxs-lookup"><span data-stu-id="a8711-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="a8711-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8711-174">Response</span></span>
<span data-ttu-id="a8711-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8711-175">The following is an example of the response.</span></span>

<span data-ttu-id="a8711-176">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a8711-176">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.bitlockerRecoveryKey)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```
