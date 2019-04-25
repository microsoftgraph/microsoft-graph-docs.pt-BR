---
title: 'bloco de anotações: getNotebookFromWebUrl'
description: Recupere as propriedades e os relacionamentos de um objeto Notebook usando seu caminho de URL.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: b5067f50b1e03c124af8323709fc7b3f70af871b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540176"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="4730e-103">bloco de anotações: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="4730e-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="4730e-104">Recupere as propriedades e os relacionamentos de um objeto [Notebook](../resources/notebook.md) usando seu caminho de URL.</span><span class="sxs-lookup"><span data-stu-id="4730e-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="4730e-105">O local pode ser blocos de anotações de usuário no Office 365, em blocos de anotações de grupo ou em blocos de anotações de equipe hospedados no site do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="4730e-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="4730e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4730e-106">Permissions</span></span>
<span data-ttu-id="4730e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4730e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4730e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4730e-109">Permission type</span></span>      | <span data-ttu-id="4730e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4730e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4730e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4730e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4730e-112">Notes. Create, Notes. Read, Notes. ReadWrite, Notes. Read. All, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4730e-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4730e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4730e-113">Application</span></span> | <span data-ttu-id="4730e-114">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4730e-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4730e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4730e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="4730e-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4730e-116">Request headers</span></span>
| <span data-ttu-id="4730e-117">Nome</span><span class="sxs-lookup"><span data-stu-id="4730e-117">Name</span></span>       | <span data-ttu-id="4730e-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="4730e-118">Type</span></span> | <span data-ttu-id="4730e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4730e-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4730e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4730e-120">Authorization</span></span>  | <span data-ttu-id="4730e-121">string</span><span class="sxs-lookup"><span data-stu-id="4730e-121">string</span></span>  | <span data-ttu-id="4730e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4730e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4730e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4730e-124">Accept</span></span> | <span data-ttu-id="4730e-125">string</span><span class="sxs-lookup"><span data-stu-id="4730e-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4730e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4730e-126">Request body</span></span>
<span data-ttu-id="4730e-127">No corpo da solicitação, forneça uma representação JSON do caminho de URL completo para o bloco de anotações que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="4730e-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="4730e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4730e-128">Property</span></span>     | <span data-ttu-id="4730e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4730e-129">Type</span></span>        | <span data-ttu-id="4730e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4730e-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="4730e-131">O caminho da URL do bloco de anotações a ser recuperado.</span><span class="sxs-lookup"><span data-stu-id="4730e-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="4730e-132">Também pode conter um prefixo "OneNote:".</span><span class="sxs-lookup"><span data-stu-id="4730e-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="4730e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4730e-133">Response</span></span>

<span data-ttu-id="4730e-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4730e-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4730e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4730e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4730e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4730e-136">Request</span></span>
<span data-ttu-id="4730e-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4730e-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="4730e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4730e-138">Response</span></span>
<span data-ttu-id="4730e-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4730e-139">Here is an example of the response.</span></span> 

><span data-ttu-id="4730e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4730e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
