---
title: Obter um usuário
description: Recuperar as propriedades e os relacionamentos do objeto user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 4568b44ac0da8727a9f6155127ab3de88c8b7029
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107847"
---
# <a name="get-a-user"></a><span data-ttu-id="a57f6-103">Obter um usuário</span><span class="sxs-lookup"><span data-stu-id="a57f6-103">Get a user</span></span>

<span data-ttu-id="a57f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a57f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a57f6-105">Recuperar as propriedades e os relacionamentos do objeto user.</span><span class="sxs-lookup"><span data-stu-id="a57f6-105">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="a57f6-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada usuário.</span><span class="sxs-lookup"><span data-stu-id="a57f6-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="a57f6-107">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="a57f6-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="a57f6-108">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](user-get.md) para o usuário e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="a57f6-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="a57f6-109">Como o recurso **usuário** dá suporte a [extensões](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **usuário**.</span><span class="sxs-lookup"><span data-stu-id="a57f6-109">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="a57f6-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a57f6-110">Permissions</span></span>
<span data-ttu-id="a57f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a57f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a57f6-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a57f6-113">Permission type</span></span>      | <span data-ttu-id="a57f6-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a57f6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a57f6-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a57f6-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a57f6-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a57f6-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a57f6-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a57f6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a57f6-118">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a57f6-118">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="a57f6-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a57f6-119">Application</span></span> | <span data-ttu-id="a57f6-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a57f6-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a57f6-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a57f6-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a57f6-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a57f6-122">Optional query parameters</span></span>
<span data-ttu-id="a57f6-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a57f6-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a57f6-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a57f6-124">Request headers</span></span>
| <span data-ttu-id="a57f6-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a57f6-125">Header</span></span>       | <span data-ttu-id="a57f6-126">Valor</span><span class="sxs-lookup"><span data-stu-id="a57f6-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="a57f6-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="a57f6-127">Authorization</span></span>  | <span data-ttu-id="a57f6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a57f6-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a57f6-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a57f6-130">Content-Type</span></span>   | <span data-ttu-id="a57f6-131">application/json</span><span class="sxs-lookup"><span data-stu-id="a57f6-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a57f6-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a57f6-132">Request body</span></span>
<span data-ttu-id="a57f6-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a57f6-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a57f6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a57f6-134">Response</span></span>

<span data-ttu-id="a57f6-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a57f6-135">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="a57f6-136">Esse método retorna `202 Accepted` quando a solicitação tenha sido processada com sucesso, mas o servidor requer mais tempo para concluir as operações de segundo plano relacionadas.</span><span class="sxs-lookup"><span data-stu-id="a57f6-136">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="a57f6-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a57f6-137">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="a57f6-138">Exemplo 1: Obter as propriedades do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="a57f6-138">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="a57f6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a57f6-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a57f6-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a57f6-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="c"></a>[<span data-ttu-id="a57f6-141">C#</span><span class="sxs-lookup"><span data-stu-id="a57f6-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a57f6-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a57f6-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a57f6-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a57f6-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a57f6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a57f6-144">Response</span></span>
<span data-ttu-id="a57f6-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a57f6-145">Here is an example of the response.</span></span> <span data-ttu-id="a57f6-146">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a57f6-146">Note: The response object shown here may be truncated for brevity.</span></span> 

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
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="a57f6-147">Exemplo 2: Obter as propriedades do usuário especificado</span><span class="sxs-lookup"><span data-stu-id="a57f6-147">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="a57f6-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a57f6-148">Request</span></span>

<span data-ttu-id="a57f6-149">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a57f6-149">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a57f6-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="a57f6-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="a57f6-151">C#</span><span class="sxs-lookup"><span data-stu-id="a57f6-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a57f6-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a57f6-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a57f6-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a57f6-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a57f6-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="a57f6-154">Response</span></span>

<span data-ttu-id="a57f6-155">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="a57f6-155">The following example shows the response.</span></span>
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
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="a57f6-156">Confira também</span><span class="sxs-lookup"><span data-stu-id="a57f6-156">See also</span></span>

- [<span data-ttu-id="a57f6-157">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="a57f6-157">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a57f6-158">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="a57f6-158">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a57f6-159">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="a57f6-159">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
