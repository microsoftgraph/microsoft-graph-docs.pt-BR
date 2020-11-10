---
title: Criar seção
description: Crie uma nova seção no grupo de seção especificado.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 7428532db09a30c6808154d1b7fe1754941e0c71
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982075"
---
# <a name="create-section"></a><span data-ttu-id="eba26-103">Criar seção</span><span class="sxs-lookup"><span data-stu-id="eba26-103">Create section</span></span>

<span data-ttu-id="eba26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eba26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eba26-105">Crie uma nova [seção](../resources/onenotesection.md) no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="eba26-105">Create a new [section](../resources/onenotesection.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="eba26-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eba26-106">Permissions</span></span>
<span data-ttu-id="eba26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eba26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eba26-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eba26-109">Permission type</span></span>      | <span data-ttu-id="eba26-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eba26-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eba26-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eba26-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eba26-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eba26-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="eba26-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eba26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eba26-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eba26-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="eba26-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eba26-115">Application</span></span> | <span data-ttu-id="eba26-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eba26-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eba26-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eba26-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sections
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
POST /groups/{id}/onenote/sectionGroups/{id}/sections
POST /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="eba26-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eba26-118">Request headers</span></span>
| <span data-ttu-id="eba26-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eba26-119">Name</span></span>       | <span data-ttu-id="eba26-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="eba26-120">Type</span></span> | <span data-ttu-id="eba26-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eba26-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eba26-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eba26-122">Authorization</span></span>  | <span data-ttu-id="eba26-123">string</span><span class="sxs-lookup"><span data-stu-id="eba26-123">string</span></span>  | <span data-ttu-id="eba26-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eba26-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eba26-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eba26-126">Content-Type</span></span> | <span data-ttu-id="eba26-127">string</span><span class="sxs-lookup"><span data-stu-id="eba26-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="eba26-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eba26-128">Request body</span></span>
<span data-ttu-id="eba26-129">No corpo da solicitação, forneça um nome para a seção.</span><span class="sxs-lookup"><span data-stu-id="eba26-129">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="eba26-p103">Dentro do mesmo nível de hierarquia, os nomes das seções devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="eba26-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="eba26-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="eba26-132">Response</span></span>

<span data-ttu-id="eba26-133">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [onenoteSection](../resources/onenotesection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eba26-133">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/onenotesection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eba26-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eba26-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eba26-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eba26-135">Request</span></span>
<span data-ttu-id="eba26-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eba26-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eba26-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="eba26-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_section_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
# <a name="c"></a>[<span data-ttu-id="eba26-138">C#</span><span class="sxs-lookup"><span data-stu-id="eba26-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-section-from-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eba26-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eba26-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-section-from-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eba26-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eba26-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-section-from-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eba26-141">Java</span><span class="sxs-lookup"><span data-stu-id="eba26-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-section-from-sectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eba26-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="eba26-142">Response</span></span>
<span data-ttu-id="eba26-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eba26-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",  
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


