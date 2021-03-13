---
title: 'notebook: getRecentNotebooks'
description: Obtenha uma lista de instâncias recentNotebook que tenham sido acessadas pelo usuário conectado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 60a2242a5f91aeaaef134fae311c511cdc2c0998
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772517"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="b03a0-103">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="b03a0-103">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="b03a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b03a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b03a0-105">Obtenha uma lista de instâncias [recentNotebook](../resources/recentnotebook.md) que tenham sido acessadas pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b03a0-105">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b03a0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b03a0-106">Permissions</span></span>
<span data-ttu-id="b03a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b03a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b03a0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b03a0-109">Permission type</span></span>      | <span data-ttu-id="b03a0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b03a0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b03a0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b03a0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b03a0-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="b03a0-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="b03a0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b03a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b03a0-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b03a0-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="b03a0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b03a0-115">Application</span></span> | <span data-ttu-id="b03a0-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b03a0-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b03a0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b03a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="b03a0-118">O `{id | userPrincipalName}` para o usuário deve corresponder ao usuário codificado no token de autorização usado para fazer a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b03a0-118">The `{id | userPrincipalName}` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="b03a0-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b03a0-119">Function parameters</span></span>

| <span data-ttu-id="b03a0-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b03a0-120">Parameter</span></span>    | <span data-ttu-id="b03a0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b03a0-121">Type</span></span>   |<span data-ttu-id="b03a0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b03a0-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b03a0-123">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="b03a0-123">includePersonalNotebooks</span></span>|<span data-ttu-id="b03a0-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="b03a0-124">Boolean</span></span>|<span data-ttu-id="b03a0-125">Inclua os blocos de anotações de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="b03a0-125">Include notebooks owned by the user.</span></span> <span data-ttu-id="b03a0-126">Defina para `true` para incluir os blocos de anotações pertencentes ao usuário; caso contrário, configure para `false`.</span><span class="sxs-lookup"><span data-stu-id="b03a0-126">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="b03a0-127">Se você não incluir o parâmetro `includePersonalNotebooks`, sua solicitação retornará uma resposta de erro `400`.</span><span class="sxs-lookup"><span data-stu-id="b03a0-127">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b03a0-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b03a0-128">Request headers</span></span>
| <span data-ttu-id="b03a0-129">Nome</span><span class="sxs-lookup"><span data-stu-id="b03a0-129">Name</span></span>       | <span data-ttu-id="b03a0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b03a0-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b03a0-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="b03a0-131">Authorization</span></span>  | <span data-ttu-id="b03a0-132">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b03a0-132">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b03a0-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b03a0-133">Request body</span></span>
<span data-ttu-id="b03a0-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b03a0-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b03a0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b03a0-135">Response</span></span>
<span data-ttu-id="b03a0-136">Uma resposta bem-sucedida retorna um `200 OK` que contém uma coleção JSON de **recentNotebooks**.</span><span class="sxs-lookup"><span data-stu-id="b03a0-136">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="b03a0-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b03a0-137">Example</span></span>
<span data-ttu-id="b03a0-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b03a0-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b03a0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b03a0-139">Request</span></span>
<span data-ttu-id="b03a0-140">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b03a0-140">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b03a0-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b03a0-141">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```
# <a name="c"></a>[<span data-ttu-id="b03a0-142">C#</span><span class="sxs-lookup"><span data-stu-id="b03a0-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/recent-notebooks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b03a0-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b03a0-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/recent-notebooks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b03a0-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b03a0-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/recent-notebooks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b03a0-145">Java</span><span class="sxs-lookup"><span data-stu-id="b03a0-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/recent-notebooks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b03a0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b03a0-146">Response</span></span>
<span data-ttu-id="b03a0-147">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="b03a0-147">The following example shows the response.</span></span>

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


