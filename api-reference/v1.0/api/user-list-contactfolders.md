---
title: Listar contactFolders
description: Obter a coleção de pastas de contatos na pasta Contatos padrão do usuário conectado.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6489b2d12cedc2cf673f4cc6493e5d815466af3b
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634462"
---
# <a name="list-contactfolders"></a><span data-ttu-id="eb5fb-103">Listar contactFolders</span><span class="sxs-lookup"><span data-stu-id="eb5fb-103">List contactFolders</span></span>

<span data-ttu-id="eb5fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb5fb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb5fb-105">Obter a coleção de pastas de contatos na pasta Contatos padrão do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="eb5fb-105">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb5fb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb5fb-106">Permissions</span></span>
<span data-ttu-id="eb5fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb5fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb5fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb5fb-109">Permission type</span></span>      | <span data-ttu-id="eb5fb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb5fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb5fb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb5fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eb5fb-112">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb5fb-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="eb5fb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb5fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb5fb-114">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb5fb-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="eb5fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb5fb-115">Application</span></span> | <span data-ttu-id="eb5fb-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb5fb-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb5fb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb5fb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eb5fb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eb5fb-118">Optional query parameters</span></span>
<span data-ttu-id="eb5fb-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eb5fb-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eb5fb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb5fb-120">Request headers</span></span>
| <span data-ttu-id="eb5fb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb5fb-121">Header</span></span>       | <span data-ttu-id="eb5fb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eb5fb-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eb5fb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb5fb-123">Authorization</span></span>  | <span data-ttu-id="eb5fb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb5fb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eb5fb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb5fb-126">Content-Type</span></span>   | <span data-ttu-id="eb5fb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="eb5fb-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eb5fb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb5fb-128">Request body</span></span>
<span data-ttu-id="eb5fb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb5fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb5fb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb5fb-130">Response</span></span>

<span data-ttu-id="eb5fb-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb5fb-131">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eb5fb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb5fb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb5fb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb5fb-133">Request</span></span>
<span data-ttu-id="eb5fb-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb5fb-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eb5fb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb5fb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders
```
# <a name="c"></a>[<span data-ttu-id="eb5fb-136">C#</span><span class="sxs-lookup"><span data-stu-id="eb5fb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb5fb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb5fb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb5fb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb5fb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb5fb-139">Java</span><span class="sxs-lookup"><span data-stu-id="eb5fb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contactfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eb5fb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb5fb-140">Response</span></span>
<span data-ttu-id="eb5fb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb5fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
