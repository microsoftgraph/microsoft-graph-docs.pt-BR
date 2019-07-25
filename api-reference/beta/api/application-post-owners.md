---
title: Criar proprietário
description: Use esta API para criar um novo proprietário.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7c7ace73e1d6a2db3bac4502f9ddae6f4f0c0e1f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856768"
---
# <a name="create-owner"></a><span data-ttu-id="c310d-103">Criar proprietário</span><span class="sxs-lookup"><span data-stu-id="c310d-103">Create owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c310d-104">Use esta API para criar um novo proprietário.</span><span class="sxs-lookup"><span data-stu-id="c310d-104">Use this API to create a new owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="c310d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c310d-105">Permissions</span></span>
<span data-ttu-id="c310d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c310d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c310d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c310d-108">Permission type</span></span>      | <span data-ttu-id="c310d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c310d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c310d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c310d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c310d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c310d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c310d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c310d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c310d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c310d-113">Not supported.</span></span>    |
|<span data-ttu-id="c310d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c310d-114">Application</span></span> | <span data-ttu-id="c310d-115">Application. ReadWrite. OwnedBy e Directory. Read. All, Application. ReadWrite. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="c310d-115">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c310d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c310d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="c310d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c310d-117">Request headers</span></span>
| <span data-ttu-id="c310d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c310d-118">Name</span></span> | <span data-ttu-id="c310d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c310d-119">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="c310d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c310d-120">Authorization</span></span> | <span data-ttu-id="c310d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c310d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c310d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c310d-123">Request body</span></span>
<span data-ttu-id="c310d-124">No corpo da solicitação, forneça o identificador do objeto de diretório a ser atribuído como proprietário.</span><span class="sxs-lookup"><span data-stu-id="c310d-124">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="c310d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c310d-125">Response</span></span>

<span data-ttu-id="c310d-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c310d-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c310d-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c310d-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="c310d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c310d-128">Request</span></span>
<span data-ttu-id="c310d-129">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c310d-129">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c310d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c310d-130">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c310d-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="c310d-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c310d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c310d-132">Response</span></span>

<span data-ttu-id="c310d-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c310d-133">The following is an example of the response.</span></span>

><span data-ttu-id="c310d-134">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c310d-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c310d-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c310d-135">All the properties will be returned from an actual call.</span></span>

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
