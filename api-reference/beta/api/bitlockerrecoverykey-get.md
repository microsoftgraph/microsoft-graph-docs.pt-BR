---
title: Obter bitlockerRecoveryKey
description: Recupere as propriedades e as relações de um objeto bitlockerRecoveryKey.
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 49c79732c2953f3e6627061b621a99c00315a4ed
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719952"
---
# <a name="get-bitlockerrecoverykey"></a><span data-ttu-id="8de2e-103">Obter bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="8de2e-103">Get bitlockerRecoveryKey</span></span>
<span data-ttu-id="8de2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8de2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8de2e-105">Recupere as propriedades e as relações de um [objeto bitlockerRecoveryKey.](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="8de2e-105">Retrieve the properties and relationships of a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object.</span></span> 

<span data-ttu-id="8de2e-106">Por padrão, essa operação não retorna a propriedade **key** que representa a chave de recuperação real.</span><span class="sxs-lookup"><span data-stu-id="8de2e-106">By default, this operation does not return the **key** property that represents the actual recovery key.</span></span> <span data-ttu-id="8de2e-107">Para incluir a **propriedade key** na resposta, use o parâmetro de `$select` consulta OData.</span><span class="sxs-lookup"><span data-stu-id="8de2e-107">To include the **key** property in the response, use the `$select` OData query parameter.</span></span> <span data-ttu-id="8de2e-108">Incluir o parâmetro de consulta dispara uma auditoria do Azure AD da operação `$select` e gera um log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="8de2e-108">Including the `$select` query parameter triggers an Azure AD audit of the operation and generates an audit log.</span></span> <span data-ttu-id="8de2e-109">Você pode encontrar o log nos logs de auditoria [do Azure AD](/azure/active-directory/reports-monitoring/concept-audit-logs) na categoria KeyManagement.</span><span class="sxs-lookup"><span data-stu-id="8de2e-109">You can find the log in [Azure AD audit logs](/azure/active-directory/reports-monitoring/concept-audit-logs) under the KeyManagement category.</span></span>

## <a name="permissions"></a><span data-ttu-id="8de2e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="8de2e-110">Permissions</span></span>
<span data-ttu-id="8de2e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8de2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8de2e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8de2e-113">Permission type</span></span>|<span data-ttu-id="8de2e-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8de2e-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8de2e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8de2e-115">Delegated (work or school account)</span></span>|<span data-ttu-id="8de2e-116">BitLocker.ReadBasic.All, BitLocker.Read.All</span><span class="sxs-lookup"><span data-stu-id="8de2e-116">BitLocker.ReadBasic.All, BitLocker.Read.All</span></span>|
|<span data-ttu-id="8de2e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8de2e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8de2e-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8de2e-118">Not supported</span></span>|
|<span data-ttu-id="8de2e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8de2e-119">Application</span></span>|<span data-ttu-id="8de2e-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8de2e-120">Not supported</span></span>|

><span data-ttu-id="8de2e-121">**Observação:** Para permissões delegadas permitirem que os aplicativos recebam recursos bitLockerRecoveryKey em nome do usuário conectado, o administrador de locatários deve ter atribuído ao usuário uma das seguintes funções ou o usuário deve ser o proprietário registrado do dispositivo do qual a chave BitLocker foi originalmente backup: </span><span class="sxs-lookup"><span data-stu-id="8de2e-121">**Note:** For delegated permissions to allow apps to get BitLockerRecoveryKey resources on behalf of the signed-in user, the tenant administrator must have assigned the user one of the following roles, or the user must be the **registered owner** of the device that the BitLocker key was originally backed up from:</span></span> 
* <span data-ttu-id="8de2e-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="8de2e-122">Global administrator</span></span>
* <span data-ttu-id="8de2e-123">Administrador de dispositivos de nuvem</span><span class="sxs-lookup"><span data-stu-id="8de2e-123">Cloud device administrator</span></span>
* <span data-ttu-id="8de2e-124">Administrador da assistência técnica</span><span class="sxs-lookup"><span data-stu-id="8de2e-124">Helpdesk administrator</span></span>
* <span data-ttu-id="8de2e-125">Administrador de Serviço do Intune</span><span class="sxs-lookup"><span data-stu-id="8de2e-125">Intune service administrator</span></span>
* <span data-ttu-id="8de2e-126">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="8de2e-126">Security administrator</span></span>
* <span data-ttu-id="8de2e-127">Leitor de segurança</span><span class="sxs-lookup"><span data-stu-id="8de2e-127">Security reader</span></span>
* <span data-ttu-id="8de2e-128">Leitor global</span><span class="sxs-lookup"><span data-stu-id="8de2e-128">Global reader</span></span>

## <a name="http-request"></a><span data-ttu-id="8de2e-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8de2e-129">HTTP request</span></span>
<span data-ttu-id="8de2e-130">Para obter a chave BitLocker especificada sem retornar a **propriedade key:**</span><span class="sxs-lookup"><span data-stu-id="8de2e-130">To get the specified BitLocker key without returning the **key** property:</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'
```

<span data-ttu-id="8de2e-131">Para obter a chave BitLocker especificada, incluindo sua **propriedade chave:**</span><span class="sxs-lookup"><span data-stu-id="8de2e-131">To get the specified BitLocker key including its **key** property:</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'?$select=key
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8de2e-132">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8de2e-132">Optional query parameters</span></span>
<span data-ttu-id="8de2e-133">Este método dá suporte ao `$select` parâmetro de consulta OData para retornar a **propriedade key.**</span><span class="sxs-lookup"><span data-stu-id="8de2e-133">This method supports the `$select` OData query parameter to return the **key** property.</span></span> <span data-ttu-id="8de2e-134">Para obter detalhes, consulte [o Exemplo 2](#example-2).</span><span class="sxs-lookup"><span data-stu-id="8de2e-134">For details, see [Example 2](#example-2).</span></span> <span data-ttu-id="8de2e-135">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8de2e-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8de2e-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8de2e-136">Request headers</span></span>
|<span data-ttu-id="8de2e-137">Nome</span><span class="sxs-lookup"><span data-stu-id="8de2e-137">Name</span></span>|<span data-ttu-id="8de2e-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="8de2e-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8de2e-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="8de2e-139">Authorization</span></span>|<span data-ttu-id="8de2e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8de2e-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8de2e-142">ocp-client-name</span><span class="sxs-lookup"><span data-stu-id="8de2e-142">ocp-client-name</span></span>|<span data-ttu-id="8de2e-143">Nome do aplicativo cliente que executa a chamada da API.</span><span class="sxs-lookup"><span data-stu-id="8de2e-143">Name of the client application performing the API call.</span></span> <span data-ttu-id="8de2e-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8de2e-144">Required.</span></span>|
|<span data-ttu-id="8de2e-145">ocp-client-version</span><span class="sxs-lookup"><span data-stu-id="8de2e-145">ocp-client-version</span></span>|<span data-ttu-id="8de2e-146">Versão do aplicativo cliente executando a chamada da API.</span><span class="sxs-lookup"><span data-stu-id="8de2e-146">Version of the client application performing the API call.</span></span> <span data-ttu-id="8de2e-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8de2e-147">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8de2e-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8de2e-148">Request body</span></span>
<span data-ttu-id="8de2e-149">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8de2e-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8de2e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8de2e-150">Response</span></span>

<span data-ttu-id="8de2e-151">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8de2e-151">If successful, this method returns a `200 OK` response code and a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8de2e-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8de2e-152">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="8de2e-153">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="8de2e-153">Example 1</span></span>
<span data-ttu-id="8de2e-154">Obter a chave BitLocker especificando a **id da chave**. Este exemplo não retorna a **propriedade key.**</span><span class="sxs-lookup"><span data-stu-id="8de2e-154">Get the BitLocker key by specifying the **key id**. This example does not return the **key** property.</span></span>

#### <a name="request"></a><span data-ttu-id="8de2e-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8de2e-155">Request</span></span>
<span data-ttu-id="8de2e-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8de2e-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8de2e-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="8de2e-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="8de2e-158">C#</span><span class="sxs-lookup"><span data-stu-id="8de2e-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8de2e-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8de2e-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8de2e-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8de2e-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8de2e-161">Java</span><span class="sxs-lookup"><span data-stu-id="8de2e-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="8de2e-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="8de2e-162">Response</span></span>
<span data-ttu-id="8de2e-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8de2e-163">The following is an example of the response.</span></span>

<span data-ttu-id="8de2e-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8de2e-164">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2"></a><span data-ttu-id="8de2e-165">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="8de2e-165">Example 2</span></span>
<span data-ttu-id="8de2e-166">Obter a chave BitLocker com a **propriedade key** especificando a **id da chave**.</span><span class="sxs-lookup"><span data-stu-id="8de2e-166">Get the BitLocker key with the **key** property by specifying the **key id**.</span></span>

#### <a name="request"></a><span data-ttu-id="8de2e-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8de2e-167">Request</span></span>
<span data-ttu-id="8de2e-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8de2e-168">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8de2e-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="8de2e-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4?$select=key
```
# <a name="c"></a>[<span data-ttu-id="8de2e-170">C#</span><span class="sxs-lookup"><span data-stu-id="8de2e-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8de2e-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8de2e-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8de2e-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8de2e-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8de2e-173">Java</span><span class="sxs-lookup"><span data-stu-id="8de2e-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="8de2e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="8de2e-174">Response</span></span>
<span data-ttu-id="8de2e-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8de2e-175">The following is an example of the response.</span></span>

<span data-ttu-id="8de2e-176">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8de2e-176">**Note:** The response object shown here might be shortened for readability.</span></span>
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
