---
title: Listar createdObjects
description: Obtenha uma lista de objetos de diretório criados pelo usuário.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d615b23fb422c8ff4007eaa7a1324ce76fc4f474
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207011"
---
# <a name="list-createdobjects"></a><span data-ttu-id="f1a32-103">Listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="f1a32-103">List createdObjects</span></span>

<span data-ttu-id="f1a32-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1a32-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1a32-105">Obtenha uma lista de objetos de diretório criados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="f1a32-105">Get a list of directory objects that were created by the user.</span></span> <span data-ttu-id="f1a32-106">Essa API retorna apenas os objetos de diretório que foram criados por um usuário que não está em nenhuma função de administrador; caso contrário, ele retorna um objeto vazio.</span><span class="sxs-lookup"><span data-stu-id="f1a32-106">This API returns only those directory objects that were created by a user who isn't in any administrator role; otherwise, it returns an empty object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1a32-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1a32-107">Permissions</span></span>
<span data-ttu-id="f1a32-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1a32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1a32-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1a32-110">Permission type</span></span>      | <span data-ttu-id="f1a32-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1a32-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1a32-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1a32-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f1a32-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1a32-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f1a32-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1a32-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1a32-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1a32-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="f1a32-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1a32-116">Application</span></span> | <span data-ttu-id="f1a32-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1a32-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="f1a32-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1a32-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
GET /me/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1a32-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1a32-119">Optional query parameters</span></span>
<span data-ttu-id="f1a32-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1a32-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f1a32-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a32-121">Request headers</span></span>
| <span data-ttu-id="f1a32-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1a32-122">Header</span></span>       | <span data-ttu-id="f1a32-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f1a32-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1a32-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1a32-124">Authorization</span></span>  | <span data-ttu-id="f1a32-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1a32-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f1a32-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1a32-127">Content-Type</span></span>  | <span data-ttu-id="f1a32-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f1a32-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1a32-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a32-129">Request body</span></span>
<span data-ttu-id="f1a32-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1a32-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1a32-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1a32-131">Response</span></span>

<span data-ttu-id="f1a32-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1a32-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1a32-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1a32-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1a32-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a32-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f1a32-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1a32-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="f1a32-136">C#</span><span class="sxs-lookup"><span data-stu-id="f1a32-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1a32-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1a32-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1a32-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1a32-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1a32-139">Java</span><span class="sxs-lookup"><span data-stu-id="f1a32-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-createdobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f1a32-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1a32-140">Response</span></span>
<span data-ttu-id="f1a32-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1a32-141">The following is an example of the response.</span></span> <span data-ttu-id="f1a32-142">A partir da resposta, o usuário criou um grupo Microsoft 365, um aplicativo e sua entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="f1a32-142">From the response, the user created a Microsoft 365 group, an application, and it's service principal.</span></span>

><span data-ttu-id="f1a32-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f1a32-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "92f3d47b-86cc-4b90-953e-8ec7f83ef45f",
      "displayName": "Contoso volunteer roster",
      "groupTypes": [
        "Unified"
      ],
      "mail": "volunteers@contoso.com",
      "mailEnabled": true,
      "mailNickname": "volunteers"
    },
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "5847962e-c746-4707-a657-f80b5b71f429",
      "appId": "254e989a-1b8c-4f8c-84e8-9dea78e9d283",
      "displayName": "ConVol",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    },
    {
      "@odata.type": "#microsoft.graph.servicePrincipal",
      "id": "ea6a54da-62be-4cdc-9860-3ed68a43d8f6",
      "accountEnabled": true,
      "appDisplayName": "ConVol",
      "appDescription": null,
      "appId": "254e989a-1b8c-4f8c-84e8-9dea78e9d283",
      "displayName": "ConVol",
      "servicePrincipalNames": [
        "254e989a-1b8c-4f8c-84e8-9dea78e9d283"
      ],
      "servicePrincipalType": "Application",
      "signInAudience": "AzureADMyOrg",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
