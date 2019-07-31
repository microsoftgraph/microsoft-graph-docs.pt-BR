---
title: Criar sectionGroup
description: Crie um novo grupo de seção no grupo da seção especificado.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 5afbb36d96d596f28f2f782f5a82ae8983a6adc6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991517"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="db62a-103">Criar sectionGroup</span><span class="sxs-lookup"><span data-stu-id="db62a-103">Create sectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db62a-104">Crie um novo [grupo de seção](../resources/sectiongroup.md) no grupo da seção especificado.</span><span class="sxs-lookup"><span data-stu-id="db62a-104">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="db62a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="db62a-105">Permissions</span></span>
<span data-ttu-id="db62a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db62a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db62a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db62a-108">Permission type</span></span>      | <span data-ttu-id="db62a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db62a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db62a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db62a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db62a-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db62a-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="db62a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db62a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db62a-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db62a-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="db62a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db62a-114">Application</span></span> | <span data-ttu-id="db62a-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db62a-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db62a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db62a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="db62a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db62a-117">Request headers</span></span>
| <span data-ttu-id="db62a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="db62a-118">Name</span></span>       | <span data-ttu-id="db62a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="db62a-119">Type</span></span> | <span data-ttu-id="db62a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="db62a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="db62a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="db62a-121">Authorization</span></span>  | <span data-ttu-id="db62a-122">string</span><span class="sxs-lookup"><span data-stu-id="db62a-122">string</span></span>  | <span data-ttu-id="db62a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db62a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db62a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db62a-125">Content-Type</span></span> | <span data-ttu-id="db62a-126">string</span><span class="sxs-lookup"><span data-stu-id="db62a-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="db62a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db62a-127">Request body</span></span>
<span data-ttu-id="db62a-128">No corpo da solicitação, forneça um nome para o grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="db62a-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="db62a-p103">Dentro do mesmo nível de hierarquia, os nomes dos grupos de seção devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="db62a-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="db62a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="db62a-131">Response</span></span>

<span data-ttu-id="db62a-132">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db62a-132">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db62a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db62a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db62a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db62a-134">Request</span></span>
<span data-ttu-id="db62a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db62a-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db62a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="db62a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db62a-137">C#</span><span class="sxs-lookup"><span data-stu-id="db62a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sectiongroup-from-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db62a-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="db62a-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sectiongroup-from-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db62a-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="db62a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sectiongroup-from-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db62a-140">Java</span><span class="sxs-lookup"><span data-stu-id="db62a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sectiongroup-from-sectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db62a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="db62a-141">Response</span></span>
<span data-ttu-id="db62a-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db62a-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
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
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
