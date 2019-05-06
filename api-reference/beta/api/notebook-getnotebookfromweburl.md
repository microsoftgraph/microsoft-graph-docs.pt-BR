---
title: 'bloco de anotações: getNotebookFromWebUrl'
description: Recupere as propriedades e os relacionamentos de um objeto Notebook usando seu caminho de URL.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 8f69fb9e2f97de7f307868b6be1a22e2e72172de
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597841"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="aedfb-103">bloco de anotações: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="aedfb-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="aedfb-104">Recupere as propriedades e os relacionamentos de um objeto [Notebook](../resources/notebook.md) usando seu caminho de URL.</span><span class="sxs-lookup"><span data-stu-id="aedfb-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="aedfb-105">O local pode ser blocos de anotações de usuário no Office 365, em blocos de anotações de grupo ou em blocos de anotações de equipe hospedados no site do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="aedfb-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="aedfb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aedfb-106">Permissions</span></span>
<span data-ttu-id="aedfb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aedfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aedfb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aedfb-109">Permission type</span></span>      | <span data-ttu-id="aedfb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aedfb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aedfb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aedfb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aedfb-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aedfb-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="aedfb-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aedfb-113">Application</span></span> | <span data-ttu-id="aedfb-114">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aedfb-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aedfb-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aedfb-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="aedfb-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aedfb-116">Request headers</span></span>
| <span data-ttu-id="aedfb-117">Nome</span><span class="sxs-lookup"><span data-stu-id="aedfb-117">Name</span></span>       | <span data-ttu-id="aedfb-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="aedfb-118">Type</span></span> | <span data-ttu-id="aedfb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="aedfb-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aedfb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="aedfb-120">Authorization</span></span>  | <span data-ttu-id="aedfb-121">string</span><span class="sxs-lookup"><span data-stu-id="aedfb-121">string</span></span>  | <span data-ttu-id="aedfb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aedfb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aedfb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aedfb-124">Accept</span></span> | <span data-ttu-id="aedfb-125">string</span><span class="sxs-lookup"><span data-stu-id="aedfb-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="aedfb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aedfb-126">Request body</span></span>
<span data-ttu-id="aedfb-127">No corpo da solicitação, forneça uma representação JSON do caminho de URL completo para o bloco de anotações que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="aedfb-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="aedfb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aedfb-128">Property</span></span>     | <span data-ttu-id="aedfb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="aedfb-129">Type</span></span>        | <span data-ttu-id="aedfb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="aedfb-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="aedfb-131">O caminho da URL do bloco de anotações a ser recuperado.</span><span class="sxs-lookup"><span data-stu-id="aedfb-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="aedfb-132">Também pode conter um prefixo "OneNote:".</span><span class="sxs-lookup"><span data-stu-id="aedfb-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="aedfb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="aedfb-133">Response</span></span>

<span data-ttu-id="aedfb-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aedfb-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aedfb-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aedfb-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aedfb-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aedfb-136">Request</span></span>
<span data-ttu-id="aedfb-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aedfb-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="aedfb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="aedfb-138">Response</span></span>
<span data-ttu-id="aedfb-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aedfb-139">Here is an example of the response.</span></span> 

><span data-ttu-id="aedfb-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aedfb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="aedfb-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="aedfb-142">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="aedfb-143">Basic</span><span class="sxs-lookup"><span data-stu-id="aedfb-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/notebook_fromweburl-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/notebook-getnotebookfromweburl.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/notebook-getnotebookfromweburl.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
