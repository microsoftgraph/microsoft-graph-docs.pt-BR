---
title: Criar sectionGroup
description: Crie um novo grupo de seção no grupo da seção especificado.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 08c519dc3b2ecd7001b89eaebf200a8506096ed7
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638820"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="5674e-103">Criar sectionGroup</span><span class="sxs-lookup"><span data-stu-id="5674e-103">Create sectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5674e-104">Crie um novo [grupo de seção](../resources/sectiongroup.md) no grupo da seção especificado.</span><span class="sxs-lookup"><span data-stu-id="5674e-104">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="5674e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5674e-105">Permissions</span></span>
<span data-ttu-id="5674e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5674e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5674e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5674e-108">Permission type</span></span>      | <span data-ttu-id="5674e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5674e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5674e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5674e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5674e-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5674e-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5674e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5674e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5674e-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5674e-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5674e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5674e-114">Application</span></span> | <span data-ttu-id="5674e-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5674e-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5674e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5674e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="5674e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5674e-117">Request headers</span></span>
| <span data-ttu-id="5674e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5674e-118">Name</span></span>       | <span data-ttu-id="5674e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="5674e-119">Type</span></span> | <span data-ttu-id="5674e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5674e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5674e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5674e-121">Authorization</span></span>  | <span data-ttu-id="5674e-122">string</span><span class="sxs-lookup"><span data-stu-id="5674e-122">string</span></span>  | <span data-ttu-id="5674e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5674e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5674e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5674e-125">Content-Type</span></span> | <span data-ttu-id="5674e-126">string</span><span class="sxs-lookup"><span data-stu-id="5674e-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5674e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5674e-127">Request body</span></span>
<span data-ttu-id="5674e-128">No corpo da solicitação, forneça um nome para o grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="5674e-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="5674e-p103">Dentro do mesmo nível de hierarquia, os nomes dos grupos de seção devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="5674e-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="5674e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5674e-131">Response</span></span>

<span data-ttu-id="5674e-132">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5674e-132">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5674e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5674e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5674e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5674e-134">Request</span></span>
<span data-ttu-id="5674e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5674e-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="5674e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5674e-136">Response</span></span>
<span data-ttu-id="5674e-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5674e-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5674e-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5674e-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5674e-141">Basic</span><span class="sxs-lookup"><span data-stu-id="5674e-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_sectiongroup_from_sectiongroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5674e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5674e-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_sectiongroup_from_sectiongroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/sectiongroup-post-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/sectiongroup-post-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
