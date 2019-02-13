---
title: 'bloco de anotações: getNotebookFromWebUrl'
description: Recupere as propriedades e relacionamentos de um objeto de bloco de anotações usando o caminho da URL.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 3d14edf5a8992f9f4386e4b50aa74d54986b62f1
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/13/2019
ms.locfileid: "29982059"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="39743-103">bloco de anotações: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="39743-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="39743-104">Recupere as propriedades e relacionamentos de um objeto de [Bloco de anotações](../resources/notebook.md) usando o caminho da URL.</span><span class="sxs-lookup"><span data-stu-id="39743-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="39743-105">O local pode ser blocos de anotações do usuário no Office 365, blocos de anotações do grupo ou blocos de anotações do SharePoint team site hospedado no Office 365.</span><span class="sxs-lookup"><span data-stu-id="39743-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="39743-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="39743-106">Permissions</span></span>
<span data-ttu-id="39743-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39743-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39743-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39743-109">Permission type</span></span>      | <span data-ttu-id="39743-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39743-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39743-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39743-111">Delegated (work or school account)</span></span> | <span data-ttu-id="39743-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39743-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="39743-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39743-113">Application</span></span> | <span data-ttu-id="39743-114">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39743-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39743-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39743-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="39743-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39743-116">Request headers</span></span>
| <span data-ttu-id="39743-117">Nome</span><span class="sxs-lookup"><span data-stu-id="39743-117">Name</span></span>       | <span data-ttu-id="39743-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="39743-118">Type</span></span> | <span data-ttu-id="39743-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="39743-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="39743-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="39743-120">Authorization</span></span>  | <span data-ttu-id="39743-121">string</span><span class="sxs-lookup"><span data-stu-id="39743-121">string</span></span>  | <span data-ttu-id="39743-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39743-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39743-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39743-124">Accept</span></span> | <span data-ttu-id="39743-125">string</span><span class="sxs-lookup"><span data-stu-id="39743-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="39743-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39743-126">Request body</span></span>
<span data-ttu-id="39743-127">No corpo da solicitação, fornece uma representação JSON do caminho URL completo para o bloco de anotações que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="39743-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="39743-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39743-128">Property</span></span>     | <span data-ttu-id="39743-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="39743-129">Type</span></span>        | <span data-ttu-id="39743-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="39743-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="39743-131">O caminho da URL de bloco de anotações para recuperar.</span><span class="sxs-lookup"><span data-stu-id="39743-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="39743-132">Ele também pode conter um "onenote:" prefixo.</span><span class="sxs-lookup"><span data-stu-id="39743-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="39743-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="39743-133">Response</span></span>

<span data-ttu-id="39743-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39743-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="39743-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39743-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39743-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39743-136">Request</span></span>
<span data-ttu-id="39743-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39743-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="39743-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="39743-138">Response</span></span>
<span data-ttu-id="39743-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39743-139">Here is an example of the response.</span></span> 

><span data-ttu-id="39743-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39743-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
