---
title: Listar recoveryKeys
description: Obter uma lista dos objetos bitlockerRecoveryKey e suas propriedades.
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a51ffa28290b51539dd8ccbcc95c71917b15db0d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944335"
---
# <a name="list-recoverykeys"></a><span data-ttu-id="38f55-103">Listar recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="38f55-103">List recoveryKeys</span></span>
<span data-ttu-id="38f55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38f55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38f55-105">Obter uma lista dos [objetos bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="38f55-105">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span> 

<span data-ttu-id="38f55-106">Esta operação não retorna a **propriedade key.**</span><span class="sxs-lookup"><span data-stu-id="38f55-106">This operation does not return the **key** property.</span></span> <span data-ttu-id="38f55-107">Para obter informações sobre como ler a **propriedade key,** consulte [Get bitlockerRecoveryKey](bitlockerrecoverykey-get.md).</span><span class="sxs-lookup"><span data-stu-id="38f55-107">For information about how to read the **key** property, see [Get bitlockerRecoveryKey](bitlockerrecoverykey-get.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="38f55-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="38f55-108">Permissions</span></span>
<span data-ttu-id="38f55-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38f55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38f55-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38f55-111">Permission type</span></span>|<span data-ttu-id="38f55-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38f55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38f55-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38f55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38f55-114">BitLocker.ReadBasic.All, BitLocker.Read.All</span><span class="sxs-lookup"><span data-stu-id="38f55-114">BitLocker.ReadBasic.All, BitLocker.Read.All</span></span>|
|<span data-ttu-id="38f55-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38f55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38f55-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="38f55-116">Not supported</span></span>|
|<span data-ttu-id="38f55-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38f55-117">Application</span></span>|<span data-ttu-id="38f55-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="38f55-118">Not supported</span></span>|

><span data-ttu-id="38f55-119">**Observação**: para permissões delegadas permitirem que os aplicativos recebam recursos do BitLockerRecoveryKey em nome do usuário conectado, o administrador de locatários deve ter atribuído ao usuário uma das seguintes funções ou o usuário deve ser o proprietário registrado do dispositivo do qual a chave de recuperação do BitLocker foi originalmente respaldada:</span><span class="sxs-lookup"><span data-stu-id="38f55-119">**Note**: For delegated permissions to allow apps to get BitLockerRecoveryKey resources on behalf of the signed-in user, the tenant administrator must have assigned the user one of the following roles, or the user must be the registered owner of the device that the BitLocker recovery key was originally backed up from:</span></span> 
* <span data-ttu-id="38f55-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="38f55-120">Global administrator</span></span>
* <span data-ttu-id="38f55-121">Administrador de dispositivos de nuvem</span><span class="sxs-lookup"><span data-stu-id="38f55-121">Cloud device administrator</span></span>
* <span data-ttu-id="38f55-122">Administrador da assistência técnica</span><span class="sxs-lookup"><span data-stu-id="38f55-122">Helpdesk administrator</span></span>
* <span data-ttu-id="38f55-123">Administrador de Serviço do Intune</span><span class="sxs-lookup"><span data-stu-id="38f55-123">Intune service administrator</span></span>
* <span data-ttu-id="38f55-124">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="38f55-124">Security administrator</span></span>
* <span data-ttu-id="38f55-125">Leitor de segurança</span><span class="sxs-lookup"><span data-stu-id="38f55-125">Security reader</span></span>
* <span data-ttu-id="38f55-126">Leitor global</span><span class="sxs-lookup"><span data-stu-id="38f55-126">Global reader</span></span>

## <a name="http-request"></a><span data-ttu-id="38f55-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38f55-127">HTTP request</span></span>
<span data-ttu-id="38f55-128">Para obter uma lista de chaves do BitLocker no locatário:</span><span class="sxs-lookup"><span data-stu-id="38f55-128">To get a list of BitLocker keys within the tenant:</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys
```

<span data-ttu-id="38f55-129">Para obter uma lista de chaves do BitLocker dentro do locatário filtrada pela **id do dispositivo**:</span><span class="sxs-lookup"><span data-stu-id="38f55-129">To get a list of BitLocker keys within the tenant filtered by the **device id**:</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys?$filter=deviceId eq '{deviceId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38f55-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="38f55-130">Optional query parameters</span></span>
<span data-ttu-id="38f55-131">Este método dá suporte ao parâmetro de consulta OData para filtrar os resultados pela id do dispositivo em que a chave foi `$filter` mais recente. </span><span class="sxs-lookup"><span data-stu-id="38f55-131">This method supports the `$filter` OData query parameter to filter results by the **device id** the key was most recently backed up to.</span></span> <span data-ttu-id="38f55-132">Este método não dá suporte ao `$top` filtro.</span><span class="sxs-lookup"><span data-stu-id="38f55-132">This method does not support the `$top` filter.</span></span> <span data-ttu-id="38f55-133">Para obter detalhes, consulte [o Exemplo 2](#example-2).</span><span class="sxs-lookup"><span data-stu-id="38f55-133">For details, see [Example 2](#example-2).</span></span> <span data-ttu-id="38f55-134">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="38f55-134">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="38f55-135">A resposta também pode conter `odata.nextLink` um , que você pode usar para página através do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="38f55-135">The response might also contain an `odata.nextLink`, which you can use to page through the result set.</span></span> <span data-ttu-id="38f55-136">Para obter detalhes, [consulte Paging Microsoft Graph data](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="38f55-136">For details, see [Paging Microsoft Graph data](/graph/paging).</span></span>

## <a name="request-headers"></a><span data-ttu-id="38f55-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38f55-137">Request headers</span></span>
|<span data-ttu-id="38f55-138">Nome</span><span class="sxs-lookup"><span data-stu-id="38f55-138">Name</span></span>|<span data-ttu-id="38f55-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="38f55-139">Description</span></span>|
|:---|:---|
|<span data-ttu-id="38f55-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="38f55-140">Authorization</span></span>|<span data-ttu-id="38f55-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38f55-p105">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="38f55-143">ocp-client-name</span><span class="sxs-lookup"><span data-stu-id="38f55-143">ocp-client-name</span></span>|<span data-ttu-id="38f55-144">Nome do aplicativo cliente que executa a chamada da API.</span><span class="sxs-lookup"><span data-stu-id="38f55-144">Name of the client application performing the API call.</span></span> <span data-ttu-id="38f55-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38f55-145">Required.</span></span>|
|<span data-ttu-id="38f55-146">ocp-client-version</span><span class="sxs-lookup"><span data-stu-id="38f55-146">ocp-client-version</span></span>|<span data-ttu-id="38f55-147">Versão do aplicativo cliente executando a chamada da API.</span><span class="sxs-lookup"><span data-stu-id="38f55-147">Version of the client application performing the API call.</span></span> <span data-ttu-id="38f55-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38f55-148">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="38f55-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38f55-149">Request body</span></span>
<span data-ttu-id="38f55-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38f55-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38f55-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="38f55-151">Response</span></span>

<span data-ttu-id="38f55-152">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38f55-152">If successful, this method returns a `200 OK` response code and a collection of [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38f55-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="38f55-153">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="38f55-154">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="38f55-154">Example 1</span></span>
<span data-ttu-id="38f55-155">Recupere uma lista de chaves do BitLocker no locatário.</span><span class="sxs-lookup"><span data-stu-id="38f55-155">Retrieve a list of BitLocker keys in the tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="38f55-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38f55-156">Request</span></span>
<span data-ttu-id="38f55-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38f55-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38f55-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="38f55-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="38f55-159">C#</span><span class="sxs-lookup"><span data-stu-id="38f55-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38f55-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38f55-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38f55-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38f55-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38f55-162">Java</span><span class="sxs-lookup"><span data-stu-id="38f55-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="38f55-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="38f55-163">Response</span></span>
<span data-ttu-id="38f55-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38f55-164">The following is an example of the response.</span></span>

<span data-ttu-id="38f55-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="38f55-165">**Note:** The response object shown here might be shortened for readability.</span></span>
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
### <a name="example-2"></a><span data-ttu-id="38f55-166">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="38f55-166">Example 2</span></span>
<span data-ttu-id="38f55-167">Recuperar uma lista de chaves BitLocker filtradas por **id de dispositivo.**</span><span class="sxs-lookup"><span data-stu-id="38f55-167">Retrieve a list of BitLocker keys filtered by **device id**.</span></span>

#### <a name="request"></a><span data-ttu-id="38f55-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38f55-168">Request</span></span>
<span data-ttu-id="38f55-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38f55-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38f55-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="38f55-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleIds": ["1ab40ab2-32a8-4b00-b6b5-ba724e407de9"],
  "name": "get_bitlockerrecoverykey_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys?$filter=deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="38f55-171">C#</span><span class="sxs-lookup"><span data-stu-id="38f55-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38f55-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38f55-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38f55-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38f55-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38f55-174">Java</span><span class="sxs-lookup"><span data-stu-id="38f55-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="38f55-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="38f55-175">Response</span></span>
<span data-ttu-id="38f55-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38f55-176">The following is an example of the response.</span></span>

<span data-ttu-id="38f55-177">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="38f55-177">**Note:** The response object shown here might be shortened for readability.</span></span>
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
