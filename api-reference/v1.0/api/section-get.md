---
title: Obter seção
description: Recupere as propriedades e relacionamentos de um objeto onenoteSection.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: d491e0936096296c731e2ebbbc1d6d44dccdef38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941552"
---
# <a name="get-section"></a><span data-ttu-id="b1338-103">Obter seção</span><span class="sxs-lookup"><span data-stu-id="b1338-103">Get section</span></span>

<span data-ttu-id="b1338-104">Recupere as propriedades e relacionamentos de um objeto [onenoteSection](../resources/section.md) .</span><span class="sxs-lookup"><span data-stu-id="b1338-104">Retrieve the properties and relationships of a [onenoteSection](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b1338-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="b1338-105">Permissions</span></span>
<span data-ttu-id="b1338-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1338-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1338-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1338-108">Permission type</span></span>      | <span data-ttu-id="b1338-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1338-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1338-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1338-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1338-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1338-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1338-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1338-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1338-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1338-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b1338-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1338-114">Application</span></span> | <span data-ttu-id="b1338-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1338-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1338-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1338-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1338-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b1338-117">Optional query parameters</span></span>
<span data-ttu-id="b1338-118">Este método dá suporte a `select` e `expand` [Parâmetros de Consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b1338-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b1338-p102">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="b1338-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1338-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1338-121">Request headers</span></span>
| <span data-ttu-id="b1338-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b1338-122">Name</span></span>       | <span data-ttu-id="b1338-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1338-123">Type</span></span> | <span data-ttu-id="b1338-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1338-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1338-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1338-125">Authorization</span></span>  | <span data-ttu-id="b1338-126">string</span><span class="sxs-lookup"><span data-stu-id="b1338-126">string</span></span>  | <span data-ttu-id="b1338-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1338-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1338-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1338-129">Accept</span></span> | <span data-ttu-id="b1338-130">string</span><span class="sxs-lookup"><span data-stu-id="b1338-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b1338-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1338-131">Request body</span></span>
<span data-ttu-id="b1338-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1338-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1338-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1338-133">Response</span></span>

<span data-ttu-id="b1338-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [onenoteSection](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1338-134">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1338-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1338-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1338-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1338-136">Request</span></span>
<span data-ttu-id="b1338-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1338-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="b1338-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1338-138">Response</span></span>
<span data-ttu-id="b1338-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1338-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
