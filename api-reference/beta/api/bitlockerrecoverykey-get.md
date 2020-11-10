---
title: Obter bitlockerRecoveryKey
description: Recupere as propriedades e os relacionamentos de um objeto bitlockerRecoveryKey.
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 72e55c0602463dcea8178935372c7f66255d98a9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960992"
---
# <a name="get-bitlockerrecoverykey"></a><span data-ttu-id="e71ad-103">Obter bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="e71ad-103">Get bitlockerRecoveryKey</span></span>
<span data-ttu-id="e71ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e71ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e71ad-105">Recupere as propriedades e os relacionamentos de um objeto [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) .</span><span class="sxs-lookup"><span data-stu-id="e71ad-105">Retrieve the properties and relationships of a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object.</span></span> 

<span data-ttu-id="e71ad-106">Por padrão, essa operação não retorna a propriedade **Key** que representa a chave de recuperação real.</span><span class="sxs-lookup"><span data-stu-id="e71ad-106">By default, this operation does not return the **key** property that represents the actual recovery key.</span></span> <span data-ttu-id="e71ad-107">Para incluir a propriedade **Key** na resposta, use o `$select` parâmetro de consulta OData.</span><span class="sxs-lookup"><span data-stu-id="e71ad-107">To include the **key** property in the response, use the `$select` OData query parameter.</span></span> <span data-ttu-id="e71ad-108">Incluindo o `$select` parâmetro de consulta dispara uma auditoria do Azure ad da operação e gera um log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="e71ad-108">Including the `$select` query parameter triggers an Azure AD audit of the operation and generates an audit log.</span></span> <span data-ttu-id="e71ad-109">Você pode encontrar o log nos [logs de auditoria do Azure ad](/azure/active-directory/reports-monitoring/concept-audit-logs) na categoria gerenciamento de Keymanagement.</span><span class="sxs-lookup"><span data-stu-id="e71ad-109">You can find the log in [Azure AD audit logs](/azure/active-directory/reports-monitoring/concept-audit-logs) under the KeyManagement category.</span></span>

## <a name="permissions"></a><span data-ttu-id="e71ad-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e71ad-110">Permissions</span></span>
<span data-ttu-id="e71ad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e71ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e71ad-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e71ad-113">Permission type</span></span>|<span data-ttu-id="e71ad-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e71ad-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e71ad-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e71ad-115">Delegated (work or school account)</span></span>|<span data-ttu-id="e71ad-116">BitLocker. ReadBasic. All, BitLocker. Read. All</span><span class="sxs-lookup"><span data-stu-id="e71ad-116">BitLocker.ReadBasic.All, BitLocker.Read.All</span></span>|
|<span data-ttu-id="e71ad-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e71ad-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e71ad-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e71ad-118">Not supported</span></span>|
|<span data-ttu-id="e71ad-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e71ad-119">Application</span></span>|<span data-ttu-id="e71ad-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e71ad-120">Not supported</span></span>|

><span data-ttu-id="e71ad-121">**Observação:** Para permissões delegadas para permitir que os aplicativos obtenham recursos do BitLockerRecoveryKey em nome do usuário conectado, o administrador do locatário deve ter atribuído o usuário uma das seguintes funções ou o usuário deve ser o **proprietário registrado** do dispositivo do qual a chave do BitLocker foi originalmente cofileirada:</span><span class="sxs-lookup"><span data-stu-id="e71ad-121">**Note:** For delegated permissions to allow apps to get BitLockerRecoveryKey resources on behalf of the signed-in user, the tenant administrator must have assigned the user one of the following roles, or the user must be the **registered owner** of the device that the BitLocker key was originally backed up from:</span></span> 
* <span data-ttu-id="e71ad-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e71ad-122">Global administrator</span></span>
* <span data-ttu-id="e71ad-123">Administrador do dispositivo de nuvem</span><span class="sxs-lookup"><span data-stu-id="e71ad-123">Cloud device administrator</span></span>
* <span data-ttu-id="e71ad-124">Administrador da assistência técnica</span><span class="sxs-lookup"><span data-stu-id="e71ad-124">Helpdesk administrator</span></span>
* <span data-ttu-id="e71ad-125">Administrador de Serviço do Intune</span><span class="sxs-lookup"><span data-stu-id="e71ad-125">Intune service administrator</span></span>
* <span data-ttu-id="e71ad-126">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="e71ad-126">Security administrator</span></span>
* <span data-ttu-id="e71ad-127">Leitor de segurança</span><span class="sxs-lookup"><span data-stu-id="e71ad-127">Security reader</span></span>
* <span data-ttu-id="e71ad-128">Leitor global</span><span class="sxs-lookup"><span data-stu-id="e71ad-128">Global reader</span></span>

## <a name="http-request"></a><span data-ttu-id="e71ad-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e71ad-129">HTTP request</span></span>
<span data-ttu-id="e71ad-130">Para obter a chave BitLocker especificada sem retornar a propriedade **Key** :</span><span class="sxs-lookup"><span data-stu-id="e71ad-130">To get the specified BitLocker key without returning the **key** property:</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'
```

<span data-ttu-id="e71ad-131">Para obter a chave BitLocker especificada, incluindo sua propriedade **Key** :</span><span class="sxs-lookup"><span data-stu-id="e71ad-131">To get the specified BitLocker key including its **key** property:</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'?$select=key
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e71ad-132">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e71ad-132">Optional query parameters</span></span>
<span data-ttu-id="e71ad-133">Este método dá suporte ao `$select` parâmetro de consulta OData para retornar a propriedade **Key** .</span><span class="sxs-lookup"><span data-stu-id="e71ad-133">This method supports the `$select` OData query parameter to return the **key** property.</span></span> <span data-ttu-id="e71ad-134">Para obter detalhes, consulte o [exemplo 2](#example-2).</span><span class="sxs-lookup"><span data-stu-id="e71ad-134">For details, see [Example 2](#example-2).</span></span> <span data-ttu-id="e71ad-135">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e71ad-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e71ad-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e71ad-136">Request headers</span></span>
|<span data-ttu-id="e71ad-137">Nome</span><span class="sxs-lookup"><span data-stu-id="e71ad-137">Name</span></span>|<span data-ttu-id="e71ad-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="e71ad-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e71ad-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="e71ad-139">Authorization</span></span>|<span data-ttu-id="e71ad-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e71ad-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e71ad-142">OCP-Client-Name</span><span class="sxs-lookup"><span data-stu-id="e71ad-142">ocp-client-name</span></span>|<span data-ttu-id="e71ad-143">Nome do aplicativo cliente executando a chamada à API.</span><span class="sxs-lookup"><span data-stu-id="e71ad-143">Name of the client application performing the API call.</span></span> <span data-ttu-id="e71ad-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e71ad-144">Required.</span></span>|
|<span data-ttu-id="e71ad-145">OCP-Client-Version</span><span class="sxs-lookup"><span data-stu-id="e71ad-145">ocp-client-version</span></span>|<span data-ttu-id="e71ad-146">Versão do aplicativo cliente executando a chamada à API.</span><span class="sxs-lookup"><span data-stu-id="e71ad-146">Version of the client application performing the API call.</span></span> <span data-ttu-id="e71ad-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e71ad-147">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e71ad-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e71ad-148">Request body</span></span>
<span data-ttu-id="e71ad-149">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e71ad-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e71ad-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e71ad-150">Response</span></span>

<span data-ttu-id="e71ad-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e71ad-151">If successful, this method returns a `200 OK` response code and a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e71ad-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e71ad-152">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="e71ad-153">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="e71ad-153">Example 1</span></span>
<span data-ttu-id="e71ad-154">Obtenha a chave do BitLocker especificando a **ID da chave**. Este exemplo não retorna a propriedade **Key** .</span><span class="sxs-lookup"><span data-stu-id="e71ad-154">Get the BitLocker key by specifying the **key id**. This example does not return the **key** property.</span></span>

#### <a name="request"></a><span data-ttu-id="e71ad-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e71ad-155">Request</span></span>
<span data-ttu-id="e71ad-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e71ad-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e71ad-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="e71ad-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="e71ad-158">C#</span><span class="sxs-lookup"><span data-stu-id="e71ad-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e71ad-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e71ad-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e71ad-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e71ad-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e71ad-161">Java</span><span class="sxs-lookup"><span data-stu-id="e71ad-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="e71ad-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="e71ad-162">Response</span></span>
<span data-ttu-id="e71ad-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e71ad-163">The following is an example of the response.</span></span>

<span data-ttu-id="e71ad-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e71ad-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
    "createdDateTime": "2020-06-15T13:45:30.0000000Z",
    "volumeType": 1,
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
  }
}
```

### <a name="example-2"></a><span data-ttu-id="e71ad-165">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="e71ad-165">Example 2</span></span>
<span data-ttu-id="e71ad-166">Obtenha a chave do BitLocker com a propriedade **Key** , especificando o **ID da chave**.</span><span class="sxs-lookup"><span data-stu-id="e71ad-166">Get the BitLocker key with the **key** property by specifying the **key id**.</span></span>

#### <a name="request"></a><span data-ttu-id="e71ad-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e71ad-167">Request</span></span>
<span data-ttu-id="e71ad-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e71ad-168">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e71ad-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="e71ad-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4?$select=key
```
# <a name="c"></a>[<span data-ttu-id="e71ad-170">C#</span><span class="sxs-lookup"><span data-stu-id="e71ad-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e71ad-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e71ad-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e71ad-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e71ad-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e71ad-173">Java</span><span class="sxs-lookup"><span data-stu-id="e71ad-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="e71ad-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="e71ad-174">Response</span></span>
<span data-ttu-id="e71ad-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e71ad-175">The following is an example of the response.</span></span>

<span data-ttu-id="e71ad-176">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e71ad-176">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
    "createdDateTime": "String (timestamp)",
    "volumeType": 1,
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
    "key": "123456-231453-873456-213546-654678-765689-123456-324565"
  }
}
```
