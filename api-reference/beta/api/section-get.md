---
title: Obter seção
description: Recupere as propriedades e os relacionamentos de um objeto section.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 51b4ec977f92d6166540f3cf4a7dbfc54651732c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513659"
---
# <a name="get-section"></a><span data-ttu-id="38eb9-103">Obter seção</span><span class="sxs-lookup"><span data-stu-id="38eb9-103">Get section</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38eb9-104">Recupere as propriedades e os relacionamentos de um objeto [section](../resources/section.md).</span><span class="sxs-lookup"><span data-stu-id="38eb9-104">Retrieve the properties and relationships of a [section](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="38eb9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="38eb9-105">Permissions</span></span>
<span data-ttu-id="38eb9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38eb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38eb9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38eb9-108">Permission type</span></span>      | <span data-ttu-id="38eb9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38eb9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38eb9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38eb9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="38eb9-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38eb9-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="38eb9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38eb9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38eb9-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38eb9-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="38eb9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38eb9-114">Application</span></span> | <span data-ttu-id="38eb9-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38eb9-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38eb9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38eb9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="38eb9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="38eb9-117">Optional query parameters</span></span>
<span data-ttu-id="38eb9-118">Este método dá suporte a `select` e `expand` [Parâmetros de Consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="38eb9-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="38eb9-p102">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="38eb9-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38eb9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38eb9-121">Request headers</span></span>
| <span data-ttu-id="38eb9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="38eb9-122">Name</span></span>       | <span data-ttu-id="38eb9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="38eb9-123">Type</span></span> | <span data-ttu-id="38eb9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="38eb9-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="38eb9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="38eb9-125">Authorization</span></span>  | <span data-ttu-id="38eb9-126">string</span><span class="sxs-lookup"><span data-stu-id="38eb9-126">string</span></span>  | <span data-ttu-id="38eb9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38eb9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38eb9-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38eb9-129">Accept</span></span> | <span data-ttu-id="38eb9-130">string</span><span class="sxs-lookup"><span data-stu-id="38eb9-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="38eb9-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38eb9-131">Request body</span></span>
<span data-ttu-id="38eb9-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38eb9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38eb9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="38eb9-133">Response</span></span>

<span data-ttu-id="38eb9-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [section](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38eb9-134">If successful, this method returns a `200 OK` response code and a [section](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38eb9-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38eb9-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38eb9-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38eb9-136">Request</span></span>
<span data-ttu-id="38eb9-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38eb9-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="38eb9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="38eb9-138">Response</span></span>
<span data-ttu-id="38eb9-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38eb9-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/section-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
