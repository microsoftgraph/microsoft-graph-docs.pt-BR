---
title: Adicionar proprietário
description: Adicione um proprietário a um aplicativo.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: b665bd0e1457234da5337683f3ff52df93cc88d4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054634"
---
# <a name="add-owner"></a><span data-ttu-id="185fb-103">Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="185fb-103">Add owner</span></span>

<span data-ttu-id="185fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="185fb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="185fb-105">Adicione um proprietário a [um aplicativo](../resources/application.md) postando na coleção owners.</span><span class="sxs-lookup"><span data-stu-id="185fb-105">Add an owner to an [application](../resources/application.md) by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="185fb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="185fb-106">Permissions</span></span>
<span data-ttu-id="185fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="185fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="185fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="185fb-109">Permission type</span></span>      | <span data-ttu-id="185fb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="185fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="185fb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="185fb-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="185fb-112">Application.ReadWrite.All e Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="185fb-112">Application.ReadWrite.All and Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="185fb-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="185fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="185fb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="185fb-114">Not supported.</span></span>    |
|<span data-ttu-id="185fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="185fb-115">Application</span></span> | <span data-ttu-id="185fb-116">Application.ReadWrite.OwnedBy e Directory.Read.All, Application.ReadWrite.All e Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="185fb-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

> <span data-ttu-id="185fb-117">**Observação:** **Application.ReadWrite.OwnedBy** não será suficiente para adicionar outro proprietário.</span><span class="sxs-lookup"><span data-stu-id="185fb-117">**Note:** **Application.ReadWrite.OwnedBy** will not be sufficient to add another owner.</span></span> <span data-ttu-id="185fb-118">Consentimento também para **Application.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="185fb-118">Consent also to **Application.ReadWrite.All**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="185fb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="185fb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="185fb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="185fb-120">Request headers</span></span>
| <span data-ttu-id="185fb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="185fb-121">Name</span></span> | <span data-ttu-id="185fb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="185fb-122">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="185fb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="185fb-123">Authorization</span></span> | <span data-ttu-id="185fb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="185fb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="185fb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="185fb-126">Request body</span></span>
<span data-ttu-id="185fb-127">No corpo da solicitação, fornece o identificador do objeto de diretório a ser atribuído como proprietário.</span><span class="sxs-lookup"><span data-stu-id="185fb-127">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="185fb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="185fb-128">Response</span></span>

<span data-ttu-id="185fb-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="185fb-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="185fb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="185fb-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="185fb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="185fb-131">Request</span></span>
<span data-ttu-id="185fb-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="185fb-132">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="185fb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="185fb-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="185fb-134">C#</span><span class="sxs-lookup"><span data-stu-id="185fb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="185fb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="185fb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="185fb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="185fb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="185fb-137">Java</span><span class="sxs-lookup"><span data-stu-id="185fb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="185fb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="185fb-138">Response</span></span>

<span data-ttu-id="185fb-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="185fb-139">The following is an example of the response.</span></span>

><span data-ttu-id="185fb-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="185fb-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

