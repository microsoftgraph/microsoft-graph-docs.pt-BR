---
title: Obter um usuário
description: Recuperar as propriedades e os relacionamentos do objeto user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 4c3024224a002a494d0d3e698c27f9ce14f6e6a9
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524719"
---
# <a name="get-a-user"></a><span data-ttu-id="49361-103">Obter um usuário</span><span class="sxs-lookup"><span data-stu-id="49361-103">Get a user</span></span>

<span data-ttu-id="49361-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49361-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49361-105">Recuperar as propriedades e os relacionamentos do objeto user.</span><span class="sxs-lookup"><span data-stu-id="49361-105">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="49361-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada usuário.</span><span class="sxs-lookup"><span data-stu-id="49361-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="49361-107">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="49361-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="49361-108">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](user-get.md) para o usuário e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="49361-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="49361-109">Como o recurso **usuário** dá suporte a [extensões](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **usuário**.</span><span class="sxs-lookup"><span data-stu-id="49361-109">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="49361-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="49361-110">Permissions</span></span>
<span data-ttu-id="49361-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49361-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49361-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49361-113">Permission type</span></span>      | <span data-ttu-id="49361-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49361-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49361-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49361-115">Delegated (work or school account)</span></span> | <span data-ttu-id="49361-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49361-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49361-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49361-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49361-118">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49361-118">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="49361-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49361-119">Application</span></span> | <span data-ttu-id="49361-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49361-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="49361-121">Chamar o ponto de extremidade `/me` exige um usuário conectado e, portanto, uma permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="49361-121">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="49361-122">Não há suporte para permissões do aplicativo ao usar o ponto de extremidade `/me`.</span><span class="sxs-lookup"><span data-stu-id="49361-122">Application permissions are not supported when using the `/me` endpoint.</span></span>

<span data-ttu-id="49361-123">Para um usuário específico:</span><span class="sxs-lookup"><span data-stu-id="49361-123">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="49361-124">Para o usuário conectado:</span><span class="sxs-lookup"><span data-stu-id="49361-124">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49361-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="49361-125">Optional query parameters</span></span>

<span data-ttu-id="49361-126">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="49361-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49361-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49361-127">Request headers</span></span>

| <span data-ttu-id="49361-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49361-128">Header</span></span>       | <span data-ttu-id="49361-129">Valor</span><span class="sxs-lookup"><span data-stu-id="49361-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="49361-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="49361-130">Authorization</span></span>  | <span data-ttu-id="49361-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49361-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="49361-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49361-133">Content-Type</span></span>   | <span data-ttu-id="49361-134">application/json</span><span class="sxs-lookup"><span data-stu-id="49361-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="49361-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49361-135">Request body</span></span>

<span data-ttu-id="49361-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49361-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49361-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="49361-137">Response</span></span>

<span data-ttu-id="49361-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49361-138">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="49361-139">Esse método retorna `202 Accepted` quando a solicitação tenha sido processada com sucesso, mas o servidor requer mais tempo para concluir as operações de segundo plano relacionadas.</span><span class="sxs-lookup"><span data-stu-id="49361-139">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="49361-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49361-140">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="49361-141">Exemplo 1: Obter as propriedades do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="49361-141">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="49361-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49361-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="49361-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="49361-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="c"></a>[<span data-ttu-id="49361-144">C#</span><span class="sxs-lookup"><span data-stu-id="49361-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49361-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49361-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49361-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49361-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49361-147">Java</span><span class="sxs-lookup"><span data-stu-id="49361-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="49361-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="49361-148">Response</span></span>
<span data-ttu-id="49361-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49361-149">Here is an example of the response.</span></span> <span data-ttu-id="49361-150">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="49361-150">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "Adele Vance",
   "givenName": "Adele",
   "jobTitle": "Retail Manager",
   "mail": "AdeleV@contoso.onmicrosoft.com",
   "mobilePhone": "+1 425 555 0109",
   "officeLocation": "18/2111",
   "preferredLanguage": "en-US",
   "surname": "Vance",
   "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
   "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
}
```

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="49361-151">Exemplo 2: Obter as propriedades do usuário especificado</span><span class="sxs-lookup"><span data-stu-id="49361-151">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="49361-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49361-152">Request</span></span>

<span data-ttu-id="49361-153">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="49361-153">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="49361-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="49361-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="49361-155">C#</span><span class="sxs-lookup"><span data-stu-id="49361-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49361-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49361-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49361-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49361-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49361-158">Java</span><span class="sxs-lookup"><span data-stu-id="49361-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49361-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="49361-159">Response</span></span>

<span data-ttu-id="49361-160">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="49361-160">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
      "displayName": "Adele Vance",
      "givenName": "Adele",
      "jobTitle": "Retail Manager",
      "mail": "AdeleV@contoso.onmicrosoft.com",
      "mobilePhone": "+1 425 555 0109",
      "officeLocation": "18/2111",
      "preferredLanguage": "en-US",
      "surname": "Vance",
      "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
      "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
}
```

## <a name="see-also"></a><span data-ttu-id="49361-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="49361-161">See also</span></span>

- [<span data-ttu-id="49361-162">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="49361-162">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="49361-163">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="49361-163">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="49361-164">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="49361-164">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
