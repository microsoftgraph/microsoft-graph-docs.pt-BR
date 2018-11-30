---
title: Criar sectionGroup
description: Crie um novo grupo de seção no grupo da seção especificado.
ms.openlocfilehash: 721c605976f39fd2401b55224e1a3235e8b5b64b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006934"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="824ee-103">Criar sectionGroup</span><span class="sxs-lookup"><span data-stu-id="824ee-103">Create sectionGroup</span></span>

<span data-ttu-id="824ee-104">Crie um novo [grupo de seção](../resources/sectiongroup.md) no grupo da seção especificado.</span><span class="sxs-lookup"><span data-stu-id="824ee-104">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="824ee-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="824ee-105">Permissions</span></span>
<span data-ttu-id="824ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="824ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="824ee-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="824ee-108">Permission type</span></span>      | <span data-ttu-id="824ee-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="824ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="824ee-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="824ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="824ee-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="824ee-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="824ee-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="824ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="824ee-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="824ee-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="824ee-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="824ee-114">Application</span></span> | <span data-ttu-id="824ee-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="824ee-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="824ee-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="824ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="824ee-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="824ee-117">Request headers</span></span>
| <span data-ttu-id="824ee-118">Nome</span><span class="sxs-lookup"><span data-stu-id="824ee-118">Name</span></span>       | <span data-ttu-id="824ee-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="824ee-119">Type</span></span> | <span data-ttu-id="824ee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="824ee-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="824ee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="824ee-121">Authorization</span></span>  | <span data-ttu-id="824ee-122">string</span><span class="sxs-lookup"><span data-stu-id="824ee-122">string</span></span>  | <span data-ttu-id="824ee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="824ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="824ee-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="824ee-125">Content-Type</span></span> | <span data-ttu-id="824ee-126">string</span><span class="sxs-lookup"><span data-stu-id="824ee-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="824ee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="824ee-127">Request body</span></span>
<span data-ttu-id="824ee-128">No corpo da solicitação, forneça um nome para o grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="824ee-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="824ee-p103">Dentro do mesmo nível de hierarquia, os nomes dos grupos de seção devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="824ee-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="824ee-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="824ee-131">Response</span></span>

<span data-ttu-id="824ee-132">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="824ee-132">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="824ee-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="824ee-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="824ee-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="824ee-134">Request</span></span>
<span data-ttu-id="824ee-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="824ee-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="824ee-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="824ee-136">Response</span></span>
<span data-ttu-id="824ee-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="824ee-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->