---
title: 'notebook: getRecentNotebooks'
description: Obtenha uma lista de instâncias recentNotebook que tenham sido acessadas pelo usuário conectado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 978b1aeecb8b65fe8fa54e053dc63488dc7b7ac9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963594"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="d4221-103">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="d4221-103">notebook: getRecentNotebooks</span></span>

> <span data-ttu-id="d4221-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d4221-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4221-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d4221-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4221-106">Obtenha uma lista de instâncias [recentNotebook](../resources/recentnotebook.md) que tenham sido acessadas pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d4221-106">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4221-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4221-107">Permissions</span></span>
<span data-ttu-id="d4221-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4221-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4221-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4221-110">Permission type</span></span>      | <span data-ttu-id="d4221-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4221-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4221-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4221-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d4221-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="d4221-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="d4221-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4221-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4221-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4221-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="d4221-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4221-116">Application</span></span> | <span data-ttu-id="d4221-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4221-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4221-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4221-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/<id | userPrincipalName>/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="d4221-119">O `<id | userPrincipalName>` para o usuário deve corresponder ao usuário codificado no token de autorização usado para fazer a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4221-119">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="d4221-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d4221-120">Function parameters</span></span>

| <span data-ttu-id="d4221-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d4221-121">Parameter</span></span>    | <span data-ttu-id="d4221-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4221-122">Type</span></span>   |<span data-ttu-id="d4221-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4221-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4221-124">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="d4221-124">includePersonalNotebooks</span></span>|<span data-ttu-id="d4221-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4221-125">Boolean</span></span>|<span data-ttu-id="d4221-126">Inclua os blocos de anotações de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="d4221-126">Include notebooks owned by the user.</span></span> <span data-ttu-id="d4221-127">Defina para `true` para incluir os blocos de anotações pertencentes ao usuário; caso contrário, configure para `false`.</span><span class="sxs-lookup"><span data-stu-id="d4221-127">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="d4221-128">Se você não incluir o parâmetro `includePersonalNotebooks`, sua solicitação retornará uma resposta de erro `400`.</span><span class="sxs-lookup"><span data-stu-id="d4221-128">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d4221-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4221-129">Request headers</span></span>
| <span data-ttu-id="d4221-130">Nome</span><span class="sxs-lookup"><span data-stu-id="d4221-130">Name</span></span>       | <span data-ttu-id="d4221-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4221-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d4221-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4221-132">Authorization</span></span>  | <span data-ttu-id="d4221-133">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d4221-133">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4221-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4221-134">Request body</span></span>
<span data-ttu-id="d4221-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4221-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4221-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4221-136">Response</span></span>
<span data-ttu-id="d4221-137">Uma resposta bem-sucedida retorna um `200 OK` que contém uma coleção JSON de **recentNotebooks**.</span><span class="sxs-lookup"><span data-stu-id="d4221-137">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="d4221-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4221-138">Example</span></span>
<span data-ttu-id="d4221-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d4221-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d4221-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4221-140">Request</span></span>
<span data-ttu-id="d4221-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4221-141">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

##### <a name="response"></a><span data-ttu-id="d4221-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4221-142">Response</span></span>
<span data-ttu-id="d4221-143">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="d4221-143">The following example shows the response.</span></span>

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
