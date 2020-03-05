---
title: 'notebook: getRecentNotebooks'
description: Obtenha uma lista de instâncias recentNotebook que tenham sido acessadas pelo usuário conectado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 9a6542c54c8b83073f10063d27f77b30bc0abdaf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456716"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="967e6-103">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="967e6-103">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="967e6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="967e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="967e6-105">Obtenha uma lista de instâncias [recentNotebook](../resources/recentnotebook.md) que tenham sido acessadas pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="967e6-105">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="967e6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="967e6-106">Permissions</span></span>
<span data-ttu-id="967e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="967e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="967e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="967e6-109">Permission type</span></span>      | <span data-ttu-id="967e6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="967e6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="967e6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="967e6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="967e6-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="967e6-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="967e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="967e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="967e6-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="967e6-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="967e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="967e6-115">Application</span></span> | <span data-ttu-id="967e6-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="967e6-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="967e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="967e6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="967e6-118">O `{id | userPrincipalName}` para o usuário deve corresponder ao usuário codificado no token de autorização usado para fazer a solicitação.</span><span class="sxs-lookup"><span data-stu-id="967e6-118">The `{id | userPrincipalName}` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="967e6-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="967e6-119">Function parameters</span></span>

| <span data-ttu-id="967e6-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="967e6-120">Parameter</span></span>    | <span data-ttu-id="967e6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="967e6-121">Type</span></span>   |<span data-ttu-id="967e6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="967e6-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="967e6-123">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="967e6-123">includePersonalNotebooks</span></span>|<span data-ttu-id="967e6-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="967e6-124">Boolean</span></span>|<span data-ttu-id="967e6-125">Inclua os blocos de anotações de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="967e6-125">Include notebooks owned by the user.</span></span> <span data-ttu-id="967e6-126">Defina para `true` para incluir os blocos de anotações pertencentes ao usuário; caso contrário, configure para `false`.</span><span class="sxs-lookup"><span data-stu-id="967e6-126">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="967e6-127">Se você não incluir o parâmetro `includePersonalNotebooks`, sua solicitação retornará uma resposta de erro `400`.</span><span class="sxs-lookup"><span data-stu-id="967e6-127">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="967e6-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="967e6-128">Request headers</span></span>
| <span data-ttu-id="967e6-129">Nome</span><span class="sxs-lookup"><span data-stu-id="967e6-129">Name</span></span>       | <span data-ttu-id="967e6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="967e6-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="967e6-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="967e6-131">Authorization</span></span>  | <span data-ttu-id="967e6-132">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="967e6-132">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="967e6-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="967e6-133">Request body</span></span>
<span data-ttu-id="967e6-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="967e6-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="967e6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="967e6-135">Response</span></span>
<span data-ttu-id="967e6-136">Uma resposta bem-sucedida retorna um `200 OK` que contém uma coleção JSON de **recentNotebooks**.</span><span class="sxs-lookup"><span data-stu-id="967e6-136">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="967e6-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="967e6-137">Example</span></span>
<span data-ttu-id="967e6-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="967e6-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="967e6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="967e6-139">Request</span></span>
<span data-ttu-id="967e6-140">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="967e6-140">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

##### <a name="response"></a><span data-ttu-id="967e6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="967e6-141">Response</span></span>
<span data-ttu-id="967e6-142">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="967e6-142">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "name":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "name":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
