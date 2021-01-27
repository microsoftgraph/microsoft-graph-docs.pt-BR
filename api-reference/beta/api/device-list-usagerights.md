---
title: Listar usageRights do dispositivo
description: Recupere uma lista de objetos usageRights para um dispositivo.
author: jeeshnair
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 73a67ecd46085c7c4369e68db5f72655cbaf395a
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013608"
---
# <a name="list-device-usagerights"></a><span data-ttu-id="fb4e7-103">Listar usageRights do dispositivo</span><span class="sxs-lookup"><span data-stu-id="fb4e7-103">List device usageRights</span></span>
<span data-ttu-id="fb4e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb4e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb4e7-105">Recupere uma lista de [objetos usageRight](../resources/usageright.md) para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb4e7-105">Retrieve a list of [usageRight](../resources/usageright.md) objects for a given device.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb4e7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb4e7-106">Permissions</span></span>
<span data-ttu-id="fb4e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb4e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb4e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb4e7-109">Permission type</span></span>|<span data-ttu-id="fb4e7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb4e7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb4e7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb4e7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb4e7-112">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb4e7-112">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="fb4e7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb4e7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb4e7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb4e7-114">Not supported.</span></span>|
|<span data-ttu-id="fb4e7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb4e7-115">Application</span></span>|<span data-ttu-id="fb4e7-116">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb4e7-116">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb4e7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb4e7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /devices/{objectId}/usageRights
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb4e7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fb4e7-118">Optional query parameters</span></span>
<span data-ttu-id="fb4e7-119">Essa API dá suporte ao $filter [de consulta OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="fb4e7-119">This API supports the $filter [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="fb4e7-120">Os seguintes padrões de $filter são suportados:</span><span class="sxs-lookup"><span data-stu-id="fb4e7-120">The following patterns of $filter are supported:</span></span>

- <span data-ttu-id="fb4e7-121">$filter = state eq 'value'</span><span class="sxs-lookup"><span data-stu-id="fb4e7-121">$filter = state eq 'value'</span></span>
- <span data-ttu-id="fb4e7-122">$filter = serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="fb4e7-122">$filter = serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="fb4e7-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="fb4e7-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="fb4e7-124">$filter = estado em ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="fb4e7-124">$filter = state in ('value1', 'value2')</span></span>
- <span data-ttu-id="fb4e7-125">$filter = serviceIdentifier em ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="fb4e7-125">$filter = serviceIdentifier in ('value1', 'value2')</span></span>
- <span data-ttu-id="fb4e7-126">$filter = estado em ('value1', 'value2') e serviceIdentifier em ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="fb4e7-126">$filter = state in ('value1', 'value2') and serviceIdentifier in ('value1', 'value2')</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb4e7-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb4e7-127">Request headers</span></span>
|<span data-ttu-id="fb4e7-128">Nome</span><span class="sxs-lookup"><span data-stu-id="fb4e7-128">Name</span></span>|<span data-ttu-id="fb4e7-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb4e7-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fb4e7-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb4e7-130">Authorization</span></span>|<span data-ttu-id="fb4e7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb4e7-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fb4e7-133">odata.maxpagesize</span><span class="sxs-lookup"><span data-stu-id="fb4e7-133">odata.maxpagesize</span></span>|<span data-ttu-id="fb4e7-134">Definir a pereferência do tamanho máximo da página de resultados.</span><span class="sxs-lookup"><span data-stu-id="fb4e7-134">Set the max result page size pereference.</span></span> <span data-ttu-id="fb4e7-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="fb4e7-135">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb4e7-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb4e7-136">Request body</span></span>
<span data-ttu-id="fb4e7-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb4e7-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb4e7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb4e7-138">Response</span></span>
<span data-ttu-id="fb4e7-139">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção [de objetos usageRight](../resources/usageright.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb4e7-139">If successful, this method returns a `200 OK` response code and a collection of [usageRight](../resources/usageright.md) objects in the response body.</span></span>

<span data-ttu-id="fb4e7-140">Além disso, se houver mais páginas na resposta, um @odata.nextLink será retornado.</span><span class="sxs-lookup"><span data-stu-id="fb4e7-140">Additionally, if there are more pages in the response an @odata.nextLink is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="fb4e7-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fb4e7-141">Examples</span></span>

### <a name="example-1-get-all-usage-rights-for-a-device"></a><span data-ttu-id="fb4e7-142">Exemplo 1: Obter todos os direitos de uso de um dispositivo</span><span class="sxs-lookup"><span data-stu-id="fb4e7-142">Example 1: Get all usage rights for a device</span></span>
 
#### <a name="request"></a><span data-ttu-id="fb4e7-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb4e7-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fb4e7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb4e7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights
```
# <a name="c"></a>[<span data-ttu-id="fb4e7-145">C#</span><span class="sxs-lookup"><span data-stu-id="fb4e7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb4e7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb4e7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb4e7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb4e7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb4e7-148">Java</span><span class="sxs-lookup"><span data-stu-id="fb4e7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fb4e7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb4e7-149">Response</span></span>
><span data-ttu-id="fb4e7-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fb4e7-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#devices('fead5c35-ebc5-47c4-a909-c43b4faf2160')/usageRights",
  "@odata.nextLink": "https://graph.microsoft.com/beta/devices/fead5c35-ebc5-47c4-a909-c43b4faf2160/usageRights?$skiptoken=W4diD29cGKX1bX",
  "value": [
    {
      "id": "99f828b9-09f2-445d-a758-b6727316dbe1",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "mscrm.f6d23ec7-255c-4bd8-8c99-dc041d5cb8b3.517f7ddd-df45-4f1c-83ec-a081a047f546",
      "state": "active"
    }
  ]
}
```

### <a name="example-2-get-usage-rights-for-a-device-with-specific-service-identifiers-and-states"></a><span data-ttu-id="fb4e7-151">Exemplo 2: Obter direitos de uso para um dispositivo com identificadores de serviço e estados específicos</span><span class="sxs-lookup"><span data-stu-id="fb4e7-151">Example 2: Get usage rights for a device with specific service identifiers and states</span></span>

#### <a name="request"></a><span data-ttu-id="fb4e7-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb4e7-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fb4e7-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb4e7-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights?$filter=state in ('active', 'suspended') and serviceIdentifier in ('ABCD')
```
# <a name="c"></a>[<span data-ttu-id="fb4e7-154">C#</span><span class="sxs-lookup"><span data-stu-id="fb4e7-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb4e7-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb4e7-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb4e7-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb4e7-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb4e7-157">Java</span><span class="sxs-lookup"><span data-stu-id="fb4e7-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fb4e7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb4e7-158">Response</span></span>
><span data-ttu-id="fb4e7-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fb4e7-159">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#devices('fead5c35-ebc5-47c4-a909-c43b4faf2160')/usageRights",
  "value": [
    {
      "id": "9905e6b1-9040-4926-b028-fdb748c359d6",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "ABCD",
      "state": "active"
    }
  ]
}
```
