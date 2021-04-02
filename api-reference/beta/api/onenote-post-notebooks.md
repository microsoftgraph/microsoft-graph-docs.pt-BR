---
title: Criar blocos de anotações
description: Crie um novo bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 5c944fb418fad689059cdc675cac4ee71a04ece7
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507707"
---
# <a name="create-notebook"></a><span data-ttu-id="eb0e6-103">Criar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="eb0e6-103">Create notebook</span></span>

<span data-ttu-id="eb0e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb0e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb0e6-105">Crie um novo bloco de [anotações](../resources/notebook.md)do OneNote.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-105">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="eb0e6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="eb0e6-106">Permissions</span></span>
<span data-ttu-id="eb0e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb0e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb0e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb0e6-109">Permission type</span></span>      | <span data-ttu-id="eb0e6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb0e6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb0e6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb0e6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eb0e6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb0e6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb0e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb0e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb0e6-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb0e6-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="eb0e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb0e6-115">Application</span></span> | <span data-ttu-id="eb0e6-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb0e6-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb0e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb0e6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="eb0e6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb0e6-118">Request headers</span></span>
| <span data-ttu-id="eb0e6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eb0e6-119">Name</span></span>       | <span data-ttu-id="eb0e6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb0e6-120">Type</span></span> | <span data-ttu-id="eb0e6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb0e6-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eb0e6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb0e6-122">Authorization</span></span>  | <span data-ttu-id="eb0e6-123">string</span><span class="sxs-lookup"><span data-stu-id="eb0e6-123">string</span></span>  | <span data-ttu-id="eb0e6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb0e6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb0e6-126">Content-Type</span></span> | <span data-ttu-id="eb0e6-127">string</span><span class="sxs-lookup"><span data-stu-id="eb0e6-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="eb0e6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb0e6-128">Request body</span></span>
<span data-ttu-id="eb0e6-129">No corpo da solicitação, fornece um nome para o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-129">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="eb0e6-130">Os nomes de bloco de anotações devem ser exclusivos.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-130">Notebook names must be unique.</span></span> <span data-ttu-id="eb0e6-131">O nome não pode conter mais de 128 caracteres ou conter os seguintes caracteres: ?\* \/ :<>|'"</span><span class="sxs-lookup"><span data-stu-id="eb0e6-131">The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="eb0e6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb0e6-132">Response</span></span>

<span data-ttu-id="eb0e6-133">Se tiver êxito, este método retornará um código `201 Created` de resposta e o novo objeto de bloco de [anotações](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-133">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb0e6-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb0e6-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb0e6-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb0e6-135">Request</span></span>
<span data-ttu-id="eb0e6-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eb0e6-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb0e6-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks
Content-type: application/json

{
    "displayName": "My Private notebook"
}
```
# <a name="c"></a>[<span data-ttu-id="eb0e6-138">C#</span><span class="sxs-lookup"><span data-stu-id="eb0e6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-notebook-from-onenote-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb0e6-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb0e6-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notebook-from-onenote-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb0e6-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb0e6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-notebook-from-onenote-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb0e6-141">Java</span><span class="sxs-lookup"><span data-stu-id="eb0e6-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-notebook-from-onenote-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb0e6-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb0e6-142">Response</span></span>
<span data-ttu-id="eb0e6-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('7d54cb02-aaa3-4016-9f9c-a4b49422dd9b')/onenote/notebooks/$entity",
    "id": "1-10143016-70dc-4449-b92a-3015225f800d",
    "self": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d",
    "displayName": "My Private notebook",
    "userRole": "Owner",
    "isShared": false,
    "sectionsUrl": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d/sections",
    "sectionGroupsUrl": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d/sectionGroups",
    "links": {
        "oneNoteClientUrl": {
            "href": "onenote:https://contoso-my.sharepoint.com/personal/admin_m365x841051_onmicrosoft_com/Documents/Notebooks/My%20Private%20notebook"
        },
        "oneNoteWebUrl": {
            "href": "https://contoso-my.sharepoint.com/personal/admin_m365x841051_onmicrosoft_com/Documents/Notebooks/My%20Private%20notebook"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


