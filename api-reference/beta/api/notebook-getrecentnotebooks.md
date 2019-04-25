---
title: 'notebook: getRecentNotebooks'
description: Obtenha uma lista de instâncias recentNotebook que tenham sido acessadas pelo usuário conectado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: a69044f908901ed0eda044eab5883f5142327e26
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540215"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="8d8cf-103">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="8d8cf-103">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="8d8cf-104">Obtenha uma lista de instâncias [recentNotebook](../resources/recentnotebook.md) que tenham sido acessadas pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8d8cf-104">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d8cf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d8cf-105">Permissions</span></span>
<span data-ttu-id="8d8cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d8cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d8cf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d8cf-108">Permission type</span></span>      | <span data-ttu-id="8d8cf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d8cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d8cf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d8cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8d8cf-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="8d8cf-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="8d8cf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d8cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d8cf-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d8cf-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="8d8cf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d8cf-114">Application</span></span> | <span data-ttu-id="8d8cf-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d8cf-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d8cf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d8cf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="8d8cf-117">O `{id | userPrincipalName}` para o usuário deve corresponder ao usuário codificado no token de autorização usado para fazer a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d8cf-117">The `{id | userPrincipalName}` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="8d8cf-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8d8cf-118">Function parameters</span></span>

| <span data-ttu-id="8d8cf-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8d8cf-119">Parameter</span></span>    | <span data-ttu-id="8d8cf-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d8cf-120">Type</span></span>   |<span data-ttu-id="8d8cf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d8cf-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d8cf-122">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="8d8cf-122">includePersonalNotebooks</span></span>|<span data-ttu-id="8d8cf-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d8cf-123">Boolean</span></span>|<span data-ttu-id="8d8cf-124">Inclua os blocos de anotações de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="8d8cf-124">Include notebooks owned by the user.</span></span> <span data-ttu-id="8d8cf-125">Defina para `true` para incluir os blocos de anotações pertencentes ao usuário; caso contrário, configure para `false`.</span><span class="sxs-lookup"><span data-stu-id="8d8cf-125">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="8d8cf-126">Se você não incluir o parâmetro `includePersonalNotebooks`, sua solicitação retornará uma resposta de erro `400`.</span><span class="sxs-lookup"><span data-stu-id="8d8cf-126">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="8d8cf-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d8cf-127">Request headers</span></span>
| <span data-ttu-id="8d8cf-128">Nome</span><span class="sxs-lookup"><span data-stu-id="8d8cf-128">Name</span></span>       | <span data-ttu-id="8d8cf-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d8cf-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d8cf-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d8cf-130">Authorization</span></span>  | <span data-ttu-id="8d8cf-131">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="8d8cf-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d8cf-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d8cf-132">Request body</span></span>
<span data-ttu-id="8d8cf-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d8cf-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d8cf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d8cf-134">Response</span></span>
<span data-ttu-id="8d8cf-135">Uma resposta bem-sucedida retorna um `200 OK` que contém uma coleção JSON de **recentNotebooks**.</span><span class="sxs-lookup"><span data-stu-id="8d8cf-135">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="8d8cf-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d8cf-136">Example</span></span>
<span data-ttu-id="8d8cf-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8d8cf-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8d8cf-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d8cf-138">Request</span></span>
<span data-ttu-id="8d8cf-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d8cf-139">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)
```

#### <a name="response"></a><span data-ttu-id="8d8cf-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d8cf-140">Response</span></span>
<span data-ttu-id="8d8cf-141">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="8d8cf-141">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.recentNotebook)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "displayName":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "displayName":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
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
