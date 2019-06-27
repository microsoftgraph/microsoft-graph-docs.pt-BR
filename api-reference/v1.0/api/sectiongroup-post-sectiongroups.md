---
title: Criar sectionGroup
description: Crie um novo grupo de seção no grupo da seção especificado.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7ed71c80959409cd5d276bc2acd7e771df4ad32a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273175"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="1c997-103">Criar sectionGroup</span><span class="sxs-lookup"><span data-stu-id="1c997-103">Create sectionGroup</span></span>

<span data-ttu-id="1c997-104">Crie um novo [grupo de seção](../resources/sectiongroup.md) no grupo da seção especificado.</span><span class="sxs-lookup"><span data-stu-id="1c997-104">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c997-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c997-105">Permissions</span></span>
<span data-ttu-id="1c997-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c997-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c997-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c997-108">Permission type</span></span>      | <span data-ttu-id="1c997-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c997-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c997-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c997-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1c997-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c997-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1c997-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c997-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c997-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c997-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1c997-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c997-114">Application</span></span> | <span data-ttu-id="1c997-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c997-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c997-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c997-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="1c997-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c997-117">Request headers</span></span>
| <span data-ttu-id="1c997-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1c997-118">Name</span></span>       | <span data-ttu-id="1c997-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c997-119">Type</span></span> | <span data-ttu-id="1c997-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c997-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1c997-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c997-121">Authorization</span></span>  | <span data-ttu-id="1c997-122">string</span><span class="sxs-lookup"><span data-stu-id="1c997-122">string</span></span>  | <span data-ttu-id="1c997-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c997-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c997-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c997-125">Content-Type</span></span> | <span data-ttu-id="1c997-126">string</span><span class="sxs-lookup"><span data-stu-id="1c997-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1c997-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c997-127">Request body</span></span>
<span data-ttu-id="1c997-128">No corpo da solicitação, forneça um nome para o grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="1c997-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="1c997-p103">Dentro do mesmo nível de hierarquia, os nomes dos grupos de seção devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="1c997-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="1c997-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c997-131">Response</span></span>

<span data-ttu-id="1c997-132">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c997-132">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c997-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c997-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c997-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c997-134">Request</span></span>
<span data-ttu-id="1c997-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c997-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
##### <a name="response"></a><span data-ttu-id="1c997-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c997-136">Response</span></span>
<span data-ttu-id="1c997-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c997-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1c997-140">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="1c997-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1c997-141">C#</span><span class="sxs-lookup"><span data-stu-id="1c997-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_sectiongroup_from_sectiongroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c997-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="1c997-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_sectiongroup_from_sectiongroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1c997-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1c997-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_sectiongroup_from_sectiongroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/sectiongroup-post-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/sectiongroup-post-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/sectiongroup-post-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
