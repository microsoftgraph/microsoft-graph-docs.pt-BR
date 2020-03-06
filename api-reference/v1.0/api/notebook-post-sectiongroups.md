---
title: Criar sectionGroup
description: Cria um novo grupo de seção no bloco de anotações especificado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 03234624efc5dd2ada63fb7b7b54c2760190a03d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511338"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="37fc4-103">Criar sectionGroup</span><span class="sxs-lookup"><span data-stu-id="37fc4-103">Create sectionGroup</span></span>

<span data-ttu-id="37fc4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37fc4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37fc4-105">Cria um novo [grupo de seção](../resources/sectiongroup.md) no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="37fc4-105">Create a new [section group](../resources/sectiongroup.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="37fc4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37fc4-106">Permissions</span></span>
<span data-ttu-id="37fc4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37fc4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37fc4-109">Permission type</span></span>      | <span data-ttu-id="37fc4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37fc4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37fc4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37fc4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37fc4-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37fc4-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="37fc4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37fc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37fc4-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37fc4-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="37fc4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37fc4-115">Application</span></span> | <span data-ttu-id="37fc4-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37fc4-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37fc4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37fc4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
POST /groups/{id}/onenote/notebooks/{id}/sectionGroups
POST /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="37fc4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37fc4-118">Request headers</span></span>
| <span data-ttu-id="37fc4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37fc4-119">Name</span></span>       | <span data-ttu-id="37fc4-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="37fc4-120">Type</span></span> | <span data-ttu-id="37fc4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="37fc4-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="37fc4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="37fc4-122">Authorization</span></span>  | <span data-ttu-id="37fc4-123">string</span><span class="sxs-lookup"><span data-stu-id="37fc4-123">string</span></span>  | <span data-ttu-id="37fc4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37fc4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37fc4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37fc4-126">Content-Type</span></span> | <span data-ttu-id="37fc4-127">string</span><span class="sxs-lookup"><span data-stu-id="37fc4-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="37fc4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37fc4-128">Request body</span></span>
<span data-ttu-id="37fc4-129">No corpo da solicitação, forneça um nome para o grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="37fc4-129">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="37fc4-p103">Dentro do mesmo nível de hierarquia, os nomes dos grupos de seção devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="37fc4-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="37fc4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="37fc4-132">Response</span></span>

<span data-ttu-id="37fc4-133">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto de objeto de [seção](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37fc4-133">If successful, this method returns `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37fc4-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37fc4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37fc4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37fc4-135">Request</span></span>
<span data-ttu-id="37fc4-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37fc4-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37fc4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="37fc4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
# <a name="c"></a>[<span data-ttu-id="37fc4-138">C#</span><span class="sxs-lookup"><span data-stu-id="37fc4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sectiongroup-from-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37fc4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37fc4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sectiongroup-from-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37fc4-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37fc4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sectiongroup-from-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37fc4-141">Java</span><span class="sxs-lookup"><span data-stu-id="37fc4-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sectiongroup-from-notebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="37fc4-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="37fc4-142">Response</span></span>
<span data-ttu-id="37fc4-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37fc4-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
