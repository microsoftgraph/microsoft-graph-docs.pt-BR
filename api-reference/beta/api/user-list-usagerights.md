---
title: Listar uso do usuárioRights
description: Recupere uma lista de objetos usageRights para um usuário.
author: jeeshnair
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2df51b15de635df52ff4b667c3a9266fafea1511
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761490"
---
# <a name="list-user-usagerights"></a><span data-ttu-id="bc225-103">Listar uso do usuárioRights</span><span class="sxs-lookup"><span data-stu-id="bc225-103">List user usageRights</span></span>
<span data-ttu-id="bc225-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc225-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc225-105">Recupere uma lista de [objetos usageRight](../resources/usageright.md) para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="bc225-105">Retrieve a list of [usageRight](../resources/usageright.md) objects for a given user.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc225-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc225-106">Permissions</span></span>
<span data-ttu-id="bc225-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc225-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc225-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc225-109">Permission type</span></span>|<span data-ttu-id="bc225-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc225-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc225-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc225-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bc225-112">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc225-112">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="bc225-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc225-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc225-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc225-114">Not supported.</span></span>|
|<span data-ttu-id="bc225-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc225-115">Application</span></span>|<span data-ttu-id="bc225-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc225-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc225-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc225-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{userId}/usageRights
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc225-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bc225-118">Optional query parameters</span></span>
<span data-ttu-id="bc225-119">Esta API dá suporte ao parâmetro $filter [consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bc225-119">This API supports the $filter [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="bc225-120">Os seguintes padrões de $filter são suportados:</span><span class="sxs-lookup"><span data-stu-id="bc225-120">The following patterns of $filter are supported:</span></span>

- <span data-ttu-id="bc225-121">$filter = estado eq 'value'</span><span class="sxs-lookup"><span data-stu-id="bc225-121">$filter = state eq 'value'</span></span>
- <span data-ttu-id="bc225-122">$filter = serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="bc225-122">$filter = serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="bc225-123">$filter = estado eq 'value' e serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="bc225-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="bc225-124">$filter = estado em ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="bc225-124">$filter = state in ('value1', 'value2')</span></span>
- <span data-ttu-id="bc225-125">$filter = serviceIdentifier em ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="bc225-125">$filter = serviceIdentifier in ('value1', 'value2')</span></span>
- <span data-ttu-id="bc225-126">$filter = estado em ('value1', 'value2') e serviceIdentifier em ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="bc225-126">$filter = state in ('value1', 'value2') and serviceIdentifier in ('value1', 'value2')</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc225-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc225-127">Request headers</span></span>
|<span data-ttu-id="bc225-128">Nome</span><span class="sxs-lookup"><span data-stu-id="bc225-128">Name</span></span>|<span data-ttu-id="bc225-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc225-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bc225-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc225-130">Authorization</span></span>|<span data-ttu-id="bc225-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc225-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bc225-133">odata.maxpagesize</span><span class="sxs-lookup"><span data-stu-id="bc225-133">odata.maxpagesize</span></span>|<span data-ttu-id="bc225-134">De definir a pereferência de tamanho máximo da página de resultados.</span><span class="sxs-lookup"><span data-stu-id="bc225-134">Set the max result page size pereference.</span></span> <span data-ttu-id="bc225-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bc225-135">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc225-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc225-136">Request body</span></span>
<span data-ttu-id="bc225-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc225-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc225-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc225-138">Response</span></span>
<span data-ttu-id="bc225-139">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [usageRight](../resources/usageright.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc225-139">If successful, this method returns a `200 OK` response code and a collection of [usageRight](../resources/usageright.md) objects in the response body.</span></span>

<span data-ttu-id="bc225-140">Além disso, se houver mais páginas na resposta, um @odata.nextLink será retornado.</span><span class="sxs-lookup"><span data-stu-id="bc225-140">Additionally, if there are more pages in the response an @odata.nextLink is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="bc225-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bc225-141">Examples</span></span>

### <a name="example-1-get-all-usage-rights-for-a-user"></a><span data-ttu-id="bc225-142">Exemplo 1: Obter todos os direitos de uso para um usuário</span><span class="sxs-lookup"><span data-stu-id="bc225-142">Example 1: Get all usage rights for a user</span></span>

#### <a name="request"></a><span data-ttu-id="bc225-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc225-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bc225-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc225-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{userId}/usageRights
```
# <a name="c"></a>[<span data-ttu-id="bc225-145">C#</span><span class="sxs-lookup"><span data-stu-id="bc225-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc225-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc225-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc225-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc225-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc225-148">Java</span><span class="sxs-lookup"><span data-stu-id="bc225-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bc225-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc225-149">Response</span></span>
><span data-ttu-id="bc225-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bc225-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-usage-rights-for-a-user-with-specific-service-identifiers-and-states"></a><span data-ttu-id="bc225-151">Exemplo 2: Obter direitos de uso para um usuário com identificadores de serviço e estados específicos</span><span class="sxs-lookup"><span data-stu-id="bc225-151">Example 2: Get usage rights for a user with specific service identifiers and states</span></span>

#### <a name="request"></a><span data-ttu-id="bc225-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc225-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bc225-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc225-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{userId}/usageRights?$filter=state in ('active', 'suspended') and serviceIdentifier in ('ABCD')
```
# <a name="c"></a>[<span data-ttu-id="bc225-154">C#</span><span class="sxs-lookup"><span data-stu-id="bc225-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc225-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc225-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc225-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc225-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc225-157">Java</span><span class="sxs-lookup"><span data-stu-id="bc225-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bc225-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc225-158">Response</span></span>
><span data-ttu-id="bc225-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bc225-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
