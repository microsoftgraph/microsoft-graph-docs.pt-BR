---
title: Criar blocos de anotações
description: Crie um novo bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: b2081f5708ba3ee0d4408120f12597ccfa71222b
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473896"
---
# <a name="create-notebook"></a><span data-ttu-id="33d99-103">Criar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="33d99-103">Create notebook</span></span>

<span data-ttu-id="33d99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33d99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33d99-105">Crie um novo bloco de [anotações](../resources/notebook.md)do OneNote.</span><span class="sxs-lookup"><span data-stu-id="33d99-105">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="33d99-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="33d99-106">Permissions</span></span>
<span data-ttu-id="33d99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33d99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33d99-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33d99-109">Permission type</span></span>      | <span data-ttu-id="33d99-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33d99-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33d99-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33d99-111">Delegated (work or school account)</span></span> | <span data-ttu-id="33d99-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33d99-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="33d99-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33d99-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33d99-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33d99-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="33d99-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33d99-115">Application</span></span> | <span data-ttu-id="33d99-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33d99-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33d99-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33d99-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="33d99-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33d99-118">Request headers</span></span>
| <span data-ttu-id="33d99-119">Nome</span><span class="sxs-lookup"><span data-stu-id="33d99-119">Name</span></span>       | <span data-ttu-id="33d99-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="33d99-120">Type</span></span> | <span data-ttu-id="33d99-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="33d99-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33d99-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="33d99-122">Authorization</span></span>  | <span data-ttu-id="33d99-123">string</span><span class="sxs-lookup"><span data-stu-id="33d99-123">string</span></span>  | <span data-ttu-id="33d99-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33d99-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33d99-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33d99-126">Content-Type</span></span> | <span data-ttu-id="33d99-127">string</span><span class="sxs-lookup"><span data-stu-id="33d99-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="33d99-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33d99-128">Request body</span></span>
<span data-ttu-id="33d99-129">No corpo da solicitação, fornece um nome para o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="33d99-129">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="33d99-130">Os nomes de bloco de anotações devem ser exclusivos.</span><span class="sxs-lookup"><span data-stu-id="33d99-130">Notebook names must be unique.</span></span> <span data-ttu-id="33d99-131">O nome não pode conter mais de 128 caracteres ou conter os seguintes caracteres: ?\* \/ :<>|'"</span><span class="sxs-lookup"><span data-stu-id="33d99-131">The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="33d99-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="33d99-132">Response</span></span>

<span data-ttu-id="33d99-133">Se tiver êxito, este método retornará um código `201 Created` de resposta e o novo objeto de bloco de [anotações](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33d99-133">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33d99-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33d99-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="33d99-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33d99-135">Request</span></span>
<span data-ttu-id="33d99-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33d99-136">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="33d99-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="33d99-137">Response</span></span>
<span data-ttu-id="33d99-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33d99-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


