---
title: Obter um usuário
description: Recuperar as propriedades e os relacionamentos do objeto user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c3bb42bd8acaecde27bb2df2e9d80eb4e2a70f3e
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275752"
---
# <a name="get-a-user"></a><span data-ttu-id="063ef-103">Obter um usuário</span><span class="sxs-lookup"><span data-stu-id="063ef-103">Get a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="063ef-104">Recuperar as propriedades e os relacionamentos do objeto user.</span><span class="sxs-lookup"><span data-stu-id="063ef-104">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="063ef-105">Como o recurso **user** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **user**.</span><span class="sxs-lookup"><span data-stu-id="063ef-105">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="063ef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="063ef-106">Permissions</span></span>
<span data-ttu-id="063ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="063ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="063ef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="063ef-109">Permission type</span></span>      | <span data-ttu-id="063ef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="063ef-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="063ef-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="063ef-111">Delegated (work or school account)</span></span> | <span data-ttu-id="063ef-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="063ef-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="063ef-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="063ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="063ef-114">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="063ef-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="063ef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="063ef-115">Application</span></span> | <span data-ttu-id="063ef-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="063ef-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="063ef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="063ef-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="063ef-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="063ef-118">Optional query parameters</span></span>
<span data-ttu-id="063ef-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="063ef-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="063ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="063ef-120">Request headers</span></span>
| <span data-ttu-id="063ef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="063ef-121">Header</span></span>       | <span data-ttu-id="063ef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="063ef-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="063ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="063ef-123">Authorization</span></span>  | <span data-ttu-id="063ef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="063ef-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="063ef-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="063ef-126">Content-Type</span></span>   | <span data-ttu-id="063ef-127">application/json</span><span class="sxs-lookup"><span data-stu-id="063ef-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="063ef-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="063ef-128">Request body</span></span>
<span data-ttu-id="063ef-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="063ef-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="063ef-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="063ef-130">Response</span></span>

<span data-ttu-id="063ef-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="063ef-131">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="063ef-132">Esse método retorna `202 Accepted` quando a solicitação tenha sido processada com sucesso, mas o servidor requer mais tempo para concluir as operações de segundo plano relacionadas.</span><span class="sxs-lookup"><span data-stu-id="063ef-132">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="063ef-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="063ef-133">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="063ef-134">Exemplo 1: Obter as propriedades do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="063ef-134">Example 1: Get the photo of the signed-in user in the largest available size</span></span>

#### <a name="request"></a><span data-ttu-id="063ef-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="063ef-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="063ef-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="063ef-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="063ef-137">C#</span><span class="sxs-lookup"><span data-stu-id="063ef-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="063ef-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="063ef-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="063ef-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="063ef-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="063ef-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="063ef-140">Response</span></span>
<span data-ttu-id="063ef-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="063ef-141">Here is an example of the response.</span></span> <span data-ttu-id="063ef-142">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="063ef-142">Note: The response object shown here may be truncated for brevity.</span></span> 

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

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="063ef-143">Exemplo 2: Obter as propriedades do usuário especificado</span><span class="sxs-lookup"><span data-stu-id="063ef-143">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="063ef-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="063ef-144">Request</span></span>

<span data-ttu-id="063ef-145">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="063ef-145">The following example shows how to create a request context.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}
```

#### <a name="response"></a><span data-ttu-id="063ef-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="063ef-146">Response</span></span>

<span data-ttu-id="063ef-147">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="063ef-147">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="063ef-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="063ef-148">See also</span></span>

- [<span data-ttu-id="063ef-149">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="063ef-149">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="063ef-150">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="063ef-150">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="063ef-151">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="063ef-151">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
