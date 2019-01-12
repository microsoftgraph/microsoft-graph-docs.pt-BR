---
title: Criar seção
description: Crie um novo onenoteSection no bloco de anotações especificado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: cec39a64f7405d13efacb1080c5d6c1482dceabb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942490"
---
# <a name="create-section"></a><span data-ttu-id="62def-103">Criar seção</span><span class="sxs-lookup"><span data-stu-id="62def-103">Create section</span></span>

<span data-ttu-id="62def-104">Crie um novo [onenoteSection](../resources/section.md) no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="62def-104">Create a new [onenoteSection](../resources/section.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="62def-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="62def-105">Permissions</span></span>
<span data-ttu-id="62def-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62def-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62def-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62def-108">Permission type</span></span>      | <span data-ttu-id="62def-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62def-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62def-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62def-110">Delegated (work or school account)</span></span> | <span data-ttu-id="62def-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62def-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="62def-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62def-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62def-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62def-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="62def-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62def-114">Application</span></span> | <span data-ttu-id="62def-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62def-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62def-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62def-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="62def-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62def-117">Request headers</span></span>
| <span data-ttu-id="62def-118">Nome</span><span class="sxs-lookup"><span data-stu-id="62def-118">Name</span></span>       | <span data-ttu-id="62def-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="62def-119">Type</span></span> | <span data-ttu-id="62def-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="62def-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="62def-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="62def-121">Authorization</span></span>  | <span data-ttu-id="62def-122">string</span><span class="sxs-lookup"><span data-stu-id="62def-122">string</span></span>  | <span data-ttu-id="62def-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62def-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="62def-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62def-125">Content-Type</span></span> | <span data-ttu-id="62def-126">string</span><span class="sxs-lookup"><span data-stu-id="62def-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="62def-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62def-127">Request body</span></span>
<span data-ttu-id="62def-128">No corpo da solicitação, forneça um nome para a seção.</span><span class="sxs-lookup"><span data-stu-id="62def-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="62def-p103">Dentro do mesmo nível de hierarquia, os nomes das seções devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="62def-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="62def-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="62def-131">Response</span></span>

<span data-ttu-id="62def-132">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [onenoteSection](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62def-132">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62def-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62def-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62def-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62def-134">Request</span></span>
<span data-ttu-id="62def-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62def-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
##### <a name="response"></a><span data-ttu-id="62def-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="62def-136">Response</span></span>
<span data-ttu-id="62def-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62def-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 201 Created
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
