---
title: Criar seção
description: Crie um novo onenoteSection do grupo da seção especificada.
localization_priority: Normal
ms.openlocfilehash: d0022c552cb24474db5cc1d7a4aa406e997ea2a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825449"
---
# <a name="create-section"></a><span data-ttu-id="8222d-103">Criar seção</span><span class="sxs-lookup"><span data-stu-id="8222d-103">Create section</span></span>

<span data-ttu-id="8222d-104">Crie um novo [onenoteSection](../resources/section.md) do grupo da seção especificada.</span><span class="sxs-lookup"><span data-stu-id="8222d-104">Create a new [onenoteSection](../resources/section.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="8222d-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="8222d-105">Permissions</span></span>
<span data-ttu-id="8222d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8222d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8222d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8222d-108">Permission type</span></span>      | <span data-ttu-id="8222d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8222d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8222d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8222d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8222d-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8222d-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="8222d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8222d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8222d-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8222d-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="8222d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8222d-114">Application</span></span> | <span data-ttu-id="8222d-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8222d-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8222d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8222d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sections
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
POST /groups/{id}/onenote/sectionGroups/{id}/sections
POST /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="8222d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8222d-117">Request headers</span></span>
| <span data-ttu-id="8222d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8222d-118">Name</span></span>       | <span data-ttu-id="8222d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8222d-119">Type</span></span> | <span data-ttu-id="8222d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8222d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8222d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8222d-121">Authorization</span></span>  | <span data-ttu-id="8222d-122">string</span><span class="sxs-lookup"><span data-stu-id="8222d-122">string</span></span>  | <span data-ttu-id="8222d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8222d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8222d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8222d-125">Content-Type</span></span> | <span data-ttu-id="8222d-126">string</span><span class="sxs-lookup"><span data-stu-id="8222d-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="8222d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8222d-127">Request body</span></span>
<span data-ttu-id="8222d-128">No corpo da solicitação, forneça um nome para a seção.</span><span class="sxs-lookup"><span data-stu-id="8222d-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="8222d-p103">Dentro do mesmo nível de hierarquia, os nomes das seções devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="8222d-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="8222d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8222d-131">Response</span></span>

<span data-ttu-id="8222d-132">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [onenoteSection](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8222d-132">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8222d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8222d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8222d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8222d-134">Request</span></span>
<span data-ttu-id="8222d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8222d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```

##### <a name="response"></a><span data-ttu-id="8222d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8222d-136">Response</span></span>
<span data-ttu-id="8222d-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8222d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
