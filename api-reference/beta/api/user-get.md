---
title: Obter um usuário
description: Recuperar as propriedades e os relacionamentos do objeto user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b0a05ee2e2bd2b4f5d2e66f5c2e0efcf27efb59
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523943"
---
# <a name="get-a-user"></a><span data-ttu-id="9402c-103">Obter um usuário</span><span class="sxs-lookup"><span data-stu-id="9402c-103">Get a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9402c-104">Recuperar as propriedades e os relacionamentos do objeto user.</span><span class="sxs-lookup"><span data-stu-id="9402c-104">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="9402c-105">Como o recurso **user** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **user**.</span><span class="sxs-lookup"><span data-stu-id="9402c-105">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="9402c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9402c-106">Permissions</span></span>
<span data-ttu-id="9402c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9402c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9402c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9402c-109">Permission type</span></span>      | <span data-ttu-id="9402c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9402c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9402c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9402c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9402c-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9402c-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9402c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9402c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9402c-114">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9402c-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="9402c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9402c-115">Application</span></span> | <span data-ttu-id="9402c-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9402c-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9402c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9402c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9402c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9402c-118">Optional query parameters</span></span>
<span data-ttu-id="9402c-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9402c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9402c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9402c-120">Request headers</span></span>
| <span data-ttu-id="9402c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9402c-121">Header</span></span>       | <span data-ttu-id="9402c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9402c-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="9402c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9402c-123">Authorization</span></span>  | <span data-ttu-id="9402c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9402c-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="9402c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9402c-126">Content-Type</span></span>   | <span data-ttu-id="9402c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9402c-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9402c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9402c-128">Request body</span></span>
<span data-ttu-id="9402c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9402c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9402c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9402c-130">Response</span></span>

<span data-ttu-id="9402c-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9402c-131">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9402c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9402c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9402c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9402c-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/me
```
##### <a name="response"></a><span data-ttu-id="9402c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9402c-134">Response</span></span>
<span data-ttu-id="9402c-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9402c-135">Here is an example of the response.</span></span> <span data-ttu-id="9402c-136">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9402c-136">Note: The response object shown here may be truncated for brevity.</span></span> 

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
  "businessPhones": [
       "businessPhones-value"
   ],
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

## <a name="see-also"></a><span data-ttu-id="9402c-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="9402c-137">See also</span></span>

- [<span data-ttu-id="9402c-138">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="9402c-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9402c-139">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="9402c-139">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="9402c-140">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="9402c-140">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/user-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
