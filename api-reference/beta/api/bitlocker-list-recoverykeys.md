---
title: Listar recoveryKeys
description: Obtenha uma lista dos objetos bitlockerRecoveryKey e suas propriedades.
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0ceadccb9ce4fbfcfffab42d403054b95c90ae50
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992559"
---
# <a name="list-recoverykeys"></a><span data-ttu-id="1608c-103">Listar recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="1608c-103">List recoveryKeys</span></span>
<span data-ttu-id="1608c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1608c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1608c-105">Obtenha uma lista dos objetos [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="1608c-105">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span> 

<span data-ttu-id="1608c-106">Essa operação não retorna a propriedade **Key** .</span><span class="sxs-lookup"><span data-stu-id="1608c-106">This operation does not return the **key** property.</span></span> <span data-ttu-id="1608c-107">Para obter informações sobre como ler a propriedade **Key** , consulte [Get bitlockerRecoveryKey](bitlockerrecoverykey-get.md).</span><span class="sxs-lookup"><span data-stu-id="1608c-107">For information about how to read the **key** property, see [Get bitlockerRecoveryKey](bitlockerrecoverykey-get.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1608c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1608c-108">Permissions</span></span>
<span data-ttu-id="1608c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1608c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1608c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1608c-111">Permission type</span></span>|<span data-ttu-id="1608c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1608c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1608c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1608c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1608c-114">BitLocker. ReadBasic. All, BitLocker. Read. All</span><span class="sxs-lookup"><span data-stu-id="1608c-114">BitLocker.ReadBasic.All, BitLocker.Read.All</span></span>|
|<span data-ttu-id="1608c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1608c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1608c-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1608c-116">Not supported</span></span>|
|<span data-ttu-id="1608c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1608c-117">Application</span></span>|<span data-ttu-id="1608c-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1608c-118">Not supported</span></span>|

><span data-ttu-id="1608c-119">**Observação**: para permissões delegadas para permitir que os aplicativos obtenham recursos do BitLockerRecoveryKey em nome do usuário conectado, o administrador do locatário deve ter atribuído ao usuário uma das seguintes funções ou o usuário deve ser o proprietário registrado do dispositivo para o qual a chave de recuperação do BitLocker foi originalmente com backup:</span><span class="sxs-lookup"><span data-stu-id="1608c-119">**Note**: For delegated permissions to allow apps to get BitLockerRecoveryKey resources on behalf of the signed-in user, the tenant administrator must have assigned the user one of the following roles, or the user must be the registered owner of the device that the BitLocker recovery key was originally backed up from:</span></span> 
* <span data-ttu-id="1608c-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1608c-120">Global administrator</span></span>
* <span data-ttu-id="1608c-121">Administrador do dispositivo de nuvem</span><span class="sxs-lookup"><span data-stu-id="1608c-121">Cloud device administrator</span></span>
* <span data-ttu-id="1608c-122">Administrador da assistência técnica</span><span class="sxs-lookup"><span data-stu-id="1608c-122">Helpdesk administrator</span></span>
* <span data-ttu-id="1608c-123">Administrador de Serviço do Intune</span><span class="sxs-lookup"><span data-stu-id="1608c-123">Intune service administrator</span></span>
* <span data-ttu-id="1608c-124">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="1608c-124">Security administrator</span></span>
* <span data-ttu-id="1608c-125">Leitor de segurança</span><span class="sxs-lookup"><span data-stu-id="1608c-125">Security reader</span></span>
* <span data-ttu-id="1608c-126">Leitor global</span><span class="sxs-lookup"><span data-stu-id="1608c-126">Global reader</span></span>

## <a name="http-request"></a><span data-ttu-id="1608c-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1608c-127">HTTP request</span></span>
<span data-ttu-id="1608c-128">Para obter uma lista de chaves do BitLocker dentro do locatário:</span><span class="sxs-lookup"><span data-stu-id="1608c-128">To get a list of BitLocker keys within the tenant:</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys
```

<span data-ttu-id="1608c-129">Para obter uma lista de chaves do BitLocker dentro do locatário filtrado pela **ID do dispositivo**:</span><span class="sxs-lookup"><span data-stu-id="1608c-129">To get a list of BitLocker keys within the tenant filtered by the **device id**:</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys?$filter=deviceId eq '{deviceId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1608c-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1608c-130">Optional query parameters</span></span>
<span data-ttu-id="1608c-131">Este método dá suporte ao `$filter` parâmetro de consulta OData para filtrar os resultados pela **ID do dispositivo** em que o backup foi feito mais recentemente.</span><span class="sxs-lookup"><span data-stu-id="1608c-131">This method supports the `$filter` OData query parameter to filter results by the **device id** the key was most recently backed up to.</span></span> <span data-ttu-id="1608c-132">Para obter detalhes, consulte o [exemplo 2](#example-2).</span><span class="sxs-lookup"><span data-stu-id="1608c-132">For details, see [Example 2](#example-2).</span></span> <span data-ttu-id="1608c-133">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1608c-133">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="1608c-134">A resposta também pode conter um `odata.nextLink` , que você pode usar para percorrer o conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="1608c-134">The response might also contain an `odata.nextLink`, which you can use to page through the result set.</span></span> <span data-ttu-id="1608c-135">Para obter detalhes, consulte [paginação de dados do Microsoft Graph](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="1608c-135">For details, see [Paging Microsoft Graph data](/graph/paging).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1608c-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1608c-136">Request headers</span></span>
|<span data-ttu-id="1608c-137">Nome</span><span class="sxs-lookup"><span data-stu-id="1608c-137">Name</span></span>|<span data-ttu-id="1608c-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="1608c-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1608c-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="1608c-139">Authorization</span></span>|<span data-ttu-id="1608c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1608c-p105">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1608c-142">OCP-Client-Name</span><span class="sxs-lookup"><span data-stu-id="1608c-142">ocp-client-name</span></span>|<span data-ttu-id="1608c-143">Nome do aplicativo cliente executando a chamada à API.</span><span class="sxs-lookup"><span data-stu-id="1608c-143">Name of the client application performing the API call.</span></span> <span data-ttu-id="1608c-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1608c-144">Required.</span></span>|
|<span data-ttu-id="1608c-145">OCP-Client-Version</span><span class="sxs-lookup"><span data-stu-id="1608c-145">ocp-client-version</span></span>|<span data-ttu-id="1608c-146">Versão do aplicativo cliente executando a chamada à API.</span><span class="sxs-lookup"><span data-stu-id="1608c-146">Version of the client application performing the API call.</span></span> <span data-ttu-id="1608c-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1608c-147">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1608c-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1608c-148">Request body</span></span>
<span data-ttu-id="1608c-149">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1608c-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1608c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1608c-150">Response</span></span>

<span data-ttu-id="1608c-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1608c-151">If successful, this method returns a `200 OK` response code and a collection of [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1608c-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1608c-152">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="1608c-153">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="1608c-153">Example 1</span></span>
<span data-ttu-id="1608c-154">Recupere uma lista de chaves do BitLocker no locatário.</span><span class="sxs-lookup"><span data-stu-id="1608c-154">Retrieve a list of BitLocker keys in the tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="1608c-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1608c-155">Request</span></span>
<span data-ttu-id="1608c-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1608c-156">The following is an example of the request.</span></span>
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


#### <a name="response"></a><span data-ttu-id="1608c-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="1608c-157">Response</span></span>
<span data-ttu-id="1608c-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1608c-158">The following is an example of the response.</span></span>

<span data-ttu-id="1608c-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1608c-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
### <a name="example-2"></a><span data-ttu-id="1608c-160">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="1608c-160">Example 2</span></span>
<span data-ttu-id="1608c-161">Recupere uma lista de chaves do BitLocker filtradas por **ID de dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="1608c-161">Retrieve a list of BitLocker keys filtered by **device id**.</span></span>

#### <a name="request"></a><span data-ttu-id="1608c-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1608c-162">Request</span></span>
<span data-ttu-id="1608c-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1608c-163">The following is an example of the request.</span></span>
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


#### <a name="response"></a><span data-ttu-id="1608c-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="1608c-164">Response</span></span>
<span data-ttu-id="1608c-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1608c-165">The following is an example of the response.</span></span>

<span data-ttu-id="1608c-166">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1608c-166">**Note:** The response object shown here might be shortened for readability.</span></span>
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
