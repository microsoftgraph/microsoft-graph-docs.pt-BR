---
title: 'bloco de anotações: getNotebookFromWebUrl'
description: Recupere as propriedades e os relacionamentos de um objeto Notebook usando seu caminho de URL.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 1d29d43bcf34c2e54651f42f3c781fdb51fc3aaf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511366"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="75a89-103">bloco de anotações: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="75a89-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="75a89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75a89-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75a89-105">Recupere as propriedades e os relacionamentos de um objeto [Notebook](../resources/notebook.md) usando seu caminho de URL.</span><span class="sxs-lookup"><span data-stu-id="75a89-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="75a89-106">O local pode ser blocos de anotações de usuário no Office 365, em blocos de anotações de grupo ou em blocos de anotações de equipe hospedados no site do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="75a89-106">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="75a89-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="75a89-107">Permissions</span></span>
<span data-ttu-id="75a89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75a89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75a89-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75a89-110">Permission type</span></span>      | <span data-ttu-id="75a89-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75a89-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75a89-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75a89-112">Delegated (work or school account)</span></span> | <span data-ttu-id="75a89-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a89-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="75a89-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a89-114">Application</span></span> | <span data-ttu-id="75a89-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a89-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75a89-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75a89-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="75a89-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75a89-117">Request headers</span></span>
| <span data-ttu-id="75a89-118">Nome</span><span class="sxs-lookup"><span data-stu-id="75a89-118">Name</span></span>       | <span data-ttu-id="75a89-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="75a89-119">Type</span></span> | <span data-ttu-id="75a89-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="75a89-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="75a89-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="75a89-121">Authorization</span></span>  | <span data-ttu-id="75a89-122">string</span><span class="sxs-lookup"><span data-stu-id="75a89-122">string</span></span>  | <span data-ttu-id="75a89-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75a89-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75a89-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75a89-125">Accept</span></span> | <span data-ttu-id="75a89-126">string</span><span class="sxs-lookup"><span data-stu-id="75a89-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="75a89-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75a89-127">Request body</span></span>
<span data-ttu-id="75a89-128">No corpo da solicitação, forneça uma representação JSON do caminho de URL completo para o bloco de anotações que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="75a89-128">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="75a89-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75a89-129">Property</span></span>     | <span data-ttu-id="75a89-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="75a89-130">Type</span></span>        | <span data-ttu-id="75a89-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="75a89-131">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="75a89-132">O caminho da URL do bloco de anotações a ser recuperado.</span><span class="sxs-lookup"><span data-stu-id="75a89-132">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="75a89-133">Também pode conter um prefixo "OneNote:".</span><span class="sxs-lookup"><span data-stu-id="75a89-133">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="75a89-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a89-134">Response</span></span>

<span data-ttu-id="75a89-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75a89-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="75a89-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75a89-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75a89-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a89-137">Request</span></span>
<span data-ttu-id="75a89-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75a89-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75a89-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="75a89-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
# <a name="c"></a>[<span data-ttu-id="75a89-140">C#</span><span class="sxs-lookup"><span data-stu-id="75a89-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-fromweburl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75a89-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75a89-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-fromweburl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75a89-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75a89-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-fromweburl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75a89-143">Java</span><span class="sxs-lookup"><span data-stu-id="75a89-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-fromweburl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="75a89-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a89-144">Response</span></span>
<span data-ttu-id="75a89-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75a89-145">Here is an example of the response.</span></span> 

><span data-ttu-id="75a89-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75a89-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json; odata.metadata=minimal
Content-Length: 544

{
    "isDefault": true,
    "userRole": "userRole-value",
    "isShared": true,
    "sectionsUrl": "sectionUrl-value",
    "sectionGroupsUrl": "sectionGroupUrl-value",
    "links": {
        "oneNoteClientUrl": {
            "href": "href-value"
        },
        "oneNoteWebUrl": {
            "href": "href-value"
        }
    },
    "id": "id-value",
    "self": "self-value",
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
