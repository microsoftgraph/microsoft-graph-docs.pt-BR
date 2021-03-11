---
title: Listar ownedObjects
description: Obtenha a lista de objetos de diretório de propriedade do usuário.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 80611733d963afe0397b8e6809621bd0cd6535b7
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718496"
---
# <a name="list-ownedobjects"></a><span data-ttu-id="20694-103">Listar ownedObjects</span><span class="sxs-lookup"><span data-stu-id="20694-103">List ownedObjects</span></span>

<span data-ttu-id="20694-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20694-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20694-105">Obtenha a lista de objetos de diretório de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="20694-105">Get the list of directory objects that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="20694-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20694-106">Permissions</span></span>
<span data-ttu-id="20694-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20694-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20694-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20694-109">Permission type</span></span>      | <span data-ttu-id="20694-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20694-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20694-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20694-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20694-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20694-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20694-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20694-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20694-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20694-114">Not supported.</span></span>    |
|<span data-ttu-id="20694-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20694-115">Application</span></span> | <span data-ttu-id="20694-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20694-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="20694-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20694-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="20694-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20694-118">Optional query parameters</span></span>
<span data-ttu-id="20694-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="20694-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="20694-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20694-120">Request headers</span></span>
| <span data-ttu-id="20694-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20694-121">Header</span></span>       | <span data-ttu-id="20694-122">Valor</span><span class="sxs-lookup"><span data-stu-id="20694-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="20694-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="20694-123">Authorization</span></span>  | <span data-ttu-id="20694-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20694-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="20694-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20694-126">Accept</span></span>  | <span data-ttu-id="20694-127">application/json</span><span class="sxs-lookup"><span data-stu-id="20694-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20694-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20694-128">Request body</span></span>
<span data-ttu-id="20694-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20694-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20694-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="20694-130">Response</span></span>

<span data-ttu-id="20694-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20694-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20694-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20694-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20694-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20694-133">Request</span></span>
<span data-ttu-id="20694-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20694-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20694-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="20694-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="20694-136">C#</span><span class="sxs-lookup"><span data-stu-id="20694-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20694-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20694-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20694-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20694-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20694-139">Java</span><span class="sxs-lookup"><span data-stu-id="20694-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ownedobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="20694-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="20694-140">Response</span></span>
<span data-ttu-id="20694-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20694-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
