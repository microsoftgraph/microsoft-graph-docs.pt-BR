---
title: Adicionar proprietário
description: Adicione um proprietário a um aplicativo.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: c4cebe3c5b35e44d5d81289dbc77cd78332350e7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958638"
---
# <a name="add-owner"></a><span data-ttu-id="3cc8e-103">Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="3cc8e-103">Add owner</span></span>

<span data-ttu-id="3cc8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cc8e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3cc8e-105">Adicione um proprietário a [um aplicativo](../resources/application.md) postando na coleção owners.</span><span class="sxs-lookup"><span data-stu-id="3cc8e-105">Add an owner to an [application](../resources/application.md) by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cc8e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cc8e-106">Permissions</span></span>
<span data-ttu-id="3cc8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cc8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cc8e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cc8e-109">Permission type</span></span>      | <span data-ttu-id="3cc8e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cc8e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cc8e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cc8e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="3cc8e-112">Application.ReadWrite.All e Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3cc8e-112">Application.ReadWrite.All and Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3cc8e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cc8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cc8e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cc8e-114">Not supported.</span></span>    |
|<span data-ttu-id="3cc8e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cc8e-115">Application</span></span> | <span data-ttu-id="3cc8e-116">Application.ReadWrite.OwnedBy e Directory.Read.All, Application.ReadWrite.All e Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cc8e-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

> <span data-ttu-id="3cc8e-117">**Observação:** **Application.ReadWrite.OwnedBy** não será suficiente para adicionar outro proprietário.</span><span class="sxs-lookup"><span data-stu-id="3cc8e-117">**Note:** **Application.ReadWrite.OwnedBy** will not be sufficient to add another owner.</span></span> <span data-ttu-id="3cc8e-118">Consentimento também para **Application.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="3cc8e-118">Consent also to **Application.ReadWrite.All**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="3cc8e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cc8e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="3cc8e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc8e-120">Request headers</span></span>
| <span data-ttu-id="3cc8e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3cc8e-121">Name</span></span> | <span data-ttu-id="3cc8e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cc8e-122">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="3cc8e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cc8e-123">Authorization</span></span> | <span data-ttu-id="3cc8e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cc8e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3cc8e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc8e-126">Request body</span></span>
<span data-ttu-id="3cc8e-127">No corpo da solicitação, fornece o identificador do objeto de diretório a ser atribuído como proprietário.</span><span class="sxs-lookup"><span data-stu-id="3cc8e-127">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="3cc8e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cc8e-128">Response</span></span>

<span data-ttu-id="3cc8e-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3cc8e-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3cc8e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cc8e-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="3cc8e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc8e-131">Request</span></span>
<span data-ttu-id="3cc8e-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cc8e-132">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3cc8e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cc8e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/v1.0/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

```
# <a name="c"></a>[<span data-ttu-id="3cc8e-134">C#</span><span class="sxs-lookup"><span data-stu-id="3cc8e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cc8e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cc8e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cc8e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cc8e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cc8e-137">Java</span><span class="sxs-lookup"><span data-stu-id="3cc8e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3cc8e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cc8e-138">Response</span></span>

<span data-ttu-id="3cc8e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3cc8e-139">The following is an example of the response.</span></span>

><span data-ttu-id="3cc8e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3cc8e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

