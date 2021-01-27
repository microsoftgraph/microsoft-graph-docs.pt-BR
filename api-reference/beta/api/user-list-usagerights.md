---
title: Listar usageRights do usuário
description: Recupere uma lista de objetos usageRights para um usuário.
author: jeeshnair
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2662458894fe6dab7fd42e0125c6b4c8f165a4e8
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013643"
---
# <a name="list-user-usagerights"></a><span data-ttu-id="224f2-103">Listar usageRights do usuário</span><span class="sxs-lookup"><span data-stu-id="224f2-103">List user usageRights</span></span>
<span data-ttu-id="224f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="224f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="224f2-105">Recupere uma lista de [objetos usageRight](../resources/usageright.md) para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="224f2-105">Retrieve a list of [usageRight](../resources/usageright.md) objects for a given user.</span></span>

## <a name="permissions"></a><span data-ttu-id="224f2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="224f2-106">Permissions</span></span>
<span data-ttu-id="224f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="224f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="224f2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="224f2-109">Permission type</span></span>|<span data-ttu-id="224f2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="224f2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="224f2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="224f2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="224f2-112">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="224f2-112">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="224f2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="224f2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="224f2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="224f2-114">Not supported.</span></span>|
|<span data-ttu-id="224f2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="224f2-115">Application</span></span>|<span data-ttu-id="224f2-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="224f2-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="224f2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="224f2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{userId}/usageRights
```

## <a name="optional-query-parameters"></a><span data-ttu-id="224f2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="224f2-118">Optional query parameters</span></span>
<span data-ttu-id="224f2-119">Essa API dá suporte ao $filter [de consulta OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="224f2-119">This API supports the $filter [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="224f2-120">Os seguintes padrões de $filter são suportados:</span><span class="sxs-lookup"><span data-stu-id="224f2-120">The following patterns of $filter are supported:</span></span>

- <span data-ttu-id="224f2-121">$filter = state eq 'value'</span><span class="sxs-lookup"><span data-stu-id="224f2-121">$filter = state eq 'value'</span></span>
- <span data-ttu-id="224f2-122">$filter = serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="224f2-122">$filter = serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="224f2-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="224f2-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="224f2-124">$filter = estado em ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="224f2-124">$filter = state in ('value1', 'value2')</span></span>
- <span data-ttu-id="224f2-125">$filter = serviceIdentifier em ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="224f2-125">$filter = serviceIdentifier in ('value1', 'value2')</span></span>
- <span data-ttu-id="224f2-126">$filter = estado em ('value1', 'value2') e serviceIdentifier em ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="224f2-126">$filter = state in ('value1', 'value2') and serviceIdentifier in ('value1', 'value2')</span></span>

## <a name="request-headers"></a><span data-ttu-id="224f2-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="224f2-127">Request headers</span></span>
|<span data-ttu-id="224f2-128">Nome</span><span class="sxs-lookup"><span data-stu-id="224f2-128">Name</span></span>|<span data-ttu-id="224f2-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="224f2-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="224f2-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="224f2-130">Authorization</span></span>|<span data-ttu-id="224f2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="224f2-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="224f2-133">odata.maxpagesize</span><span class="sxs-lookup"><span data-stu-id="224f2-133">odata.maxpagesize</span></span>|<span data-ttu-id="224f2-134">Definir a pereferência do tamanho máximo da página de resultados.</span><span class="sxs-lookup"><span data-stu-id="224f2-134">Set the max result page size pereference.</span></span> <span data-ttu-id="224f2-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="224f2-135">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="224f2-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="224f2-136">Request body</span></span>
<span data-ttu-id="224f2-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="224f2-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="224f2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="224f2-138">Response</span></span>
<span data-ttu-id="224f2-139">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção [de objetos usageRight](../resources/usageright.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="224f2-139">If successful, this method returns a `200 OK` response code and a collection of [usageRight](../resources/usageright.md) objects in the response body.</span></span>

<span data-ttu-id="224f2-140">Além disso, se houver mais páginas na resposta, um @odata.nextLink será retornado.</span><span class="sxs-lookup"><span data-stu-id="224f2-140">Additionally, if there are more pages in the response an @odata.nextLink is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="224f2-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="224f2-141">Examples</span></span>

### <a name="example-1-get-all-usage-rights-for-a-user"></a><span data-ttu-id="224f2-142">Exemplo 1: Obter todos os direitos de uso de um usuário</span><span class="sxs-lookup"><span data-stu-id="224f2-142">Example 1: Get all usage rights for a user</span></span>

#### <a name="request"></a><span data-ttu-id="224f2-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="224f2-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="224f2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="224f2-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{userId}/usageRights
```
# <a name="c"></a>[<span data-ttu-id="224f2-145">C#</span><span class="sxs-lookup"><span data-stu-id="224f2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="224f2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="224f2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="224f2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="224f2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="224f2-148">Java</span><span class="sxs-lookup"><span data-stu-id="224f2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="224f2-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="224f2-149">Response</span></span>
><span data-ttu-id="224f2-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="224f2-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64952b80-51fd-4378-9ba5-589a840afb80')/usageRights",
  "@odata.nextLink": "https://graph.microsoft.com/beta/users/64952b80-51fd-4378-9ba5-589a840afb80/usageRights?$skiptoken=W4diD29cGKX1bX",
  "value": [
    {
      "id": "c2e034cb-3cbc-41be-a496-bfcd031e4cfc",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "mscrm.f6d23ec7-255c-4bd8-8c99-dc041d5cb8b3.517f7ddd-df45-4f1c-83ec-a081a047f546",
      "state": "active"
    }
  ]
}
```

### <a name="example-2-get-usage-rights-for-a-user-with-specific-service-identifiers-and-states"></a><span data-ttu-id="224f2-151">Exemplo 2: Obter direitos de uso para um usuário com identificadores de serviço e estados específicos</span><span class="sxs-lookup"><span data-stu-id="224f2-151">Example 2: Get usage rights for a user with specific service identifiers and states</span></span>

#### <a name="request"></a><span data-ttu-id="224f2-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="224f2-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="224f2-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="224f2-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{userId}/usageRights?$filter=state in ('active', 'suspended') and serviceIdentifier in ('ABCD')
```
# <a name="c"></a>[<span data-ttu-id="224f2-154">C#</span><span class="sxs-lookup"><span data-stu-id="224f2-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="224f2-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="224f2-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="224f2-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="224f2-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="224f2-157">Java</span><span class="sxs-lookup"><span data-stu-id="224f2-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="224f2-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="224f2-158">Response</span></span>
><span data-ttu-id="224f2-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="224f2-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64952b80-51fd-4378-9ba5-589a840afb80')/usageRights",
  "value": [
    {
      "id": "505261eb-b4ee-421c-8206-05529ae2c150",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "ABCD",
      "state": "active"
    }
  ]
}
```
