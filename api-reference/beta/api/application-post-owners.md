---
title: Adicionar proprietário
description: Use essa API para adicionar um proprietário a um aplicativo.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 95642607e2a43797683f494807fb47a147216c28
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048075"
---
# <a name="add-owner"></a><span data-ttu-id="2fd7e-103">Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="2fd7e-103">Add owner</span></span>

<span data-ttu-id="2fd7e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fd7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fd7e-105">Use essa API para adicionar um proprietário a um aplicativo postando na coleção owners.</span><span class="sxs-lookup"><span data-stu-id="2fd7e-105">Use this API to add an owner to an application by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fd7e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fd7e-106">Permissions</span></span>
<span data-ttu-id="2fd7e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fd7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fd7e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fd7e-109">Permission type</span></span>      | <span data-ttu-id="2fd7e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fd7e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fd7e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fd7e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="2fd7e-112">Application.ReadWrite.All e Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2fd7e-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2fd7e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fd7e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fd7e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fd7e-114">Not supported.</span></span>    |
|<span data-ttu-id="2fd7e-115">Application</span><span class="sxs-lookup"><span data-stu-id="2fd7e-115">Application</span></span> | <span data-ttu-id="2fd7e-116">Application.ReadWrite.OwnedBy e Directory.Read.All, Application.ReadWrite.All e Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fd7e-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fd7e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fd7e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="2fd7e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fd7e-118">Request headers</span></span>
| <span data-ttu-id="2fd7e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2fd7e-119">Name</span></span> | <span data-ttu-id="2fd7e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fd7e-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="2fd7e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fd7e-121">Authorization</span></span> | <span data-ttu-id="2fd7e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fd7e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2fd7e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fd7e-124">Request body</span></span>
<span data-ttu-id="2fd7e-125">No corpo da solicitação, fornece o identificador do objeto de diretório a ser atribuído como proprietário.</span><span class="sxs-lookup"><span data-stu-id="2fd7e-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="2fd7e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fd7e-126">Response</span></span>

<span data-ttu-id="2fd7e-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2fd7e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2fd7e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fd7e-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="2fd7e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fd7e-129">Request</span></span>
<span data-ttu-id="2fd7e-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fd7e-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2fd7e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fd7e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
"@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

```
# <a name="javascript"></a>[<span data-ttu-id="2fd7e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fd7e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2fd7e-133">C#</span><span class="sxs-lookup"><span data-stu-id="2fd7e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fd7e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fd7e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2fd7e-135">Java</span><span class="sxs-lookup"><span data-stu-id="2fd7e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2fd7e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fd7e-136">Response</span></span>

<span data-ttu-id="2fd7e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2fd7e-137">The following is an example of the response.</span></span>

><span data-ttu-id="2fd7e-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2fd7e-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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



