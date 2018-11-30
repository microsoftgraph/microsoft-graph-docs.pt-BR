---
title: Listar seções
description: Recupere uma lista de objetos onenoteSection.
ms.openlocfilehash: ab6ee09acba2c6c0d30c02925e199af4484914ad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007317"
---
# <a name="list-sections"></a><span data-ttu-id="8dca3-103">Listar seções</span><span class="sxs-lookup"><span data-stu-id="8dca3-103">List sections</span></span>

<span data-ttu-id="8dca3-104">Recupere uma lista de objetos [onenoteSection](../resources/section.md) .</span><span class="sxs-lookup"><span data-stu-id="8dca3-104">Retrieve a list of [onenoteSection](../resources/section.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8dca3-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="8dca3-105">Permissions</span></span>
<span data-ttu-id="8dca3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dca3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dca3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8dca3-108">Permission type</span></span>      | <span data-ttu-id="8dca3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8dca3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dca3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8dca3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8dca3-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dca3-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="8dca3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8dca3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dca3-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8dca3-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="8dca3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8dca3-114">Application</span></span> | <span data-ttu-id="8dca3-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dca3-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dca3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8dca3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections
GET /users/{id | userPrincipalName}/onenote/sections
GET /groups/{id}/onenote/sections
GET /sites/{id}/onenote/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8dca3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8dca3-117">Optional query parameters</span></span>
<span data-ttu-id="8dca3-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8dca3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="8dca3-119">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="8dca3-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="8dca3-p102">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="8dca3-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8dca3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8dca3-122">Request headers</span></span>
| <span data-ttu-id="8dca3-123">Nome</span><span class="sxs-lookup"><span data-stu-id="8dca3-123">Name</span></span>       | <span data-ttu-id="8dca3-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dca3-124">Type</span></span> | <span data-ttu-id="8dca3-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dca3-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8dca3-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8dca3-126">Authorization</span></span>  | <span data-ttu-id="8dca3-127">string</span><span class="sxs-lookup"><span data-stu-id="8dca3-127">string</span></span>  | <span data-ttu-id="8dca3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8dca3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8dca3-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8dca3-130">Accept</span></span> | <span data-ttu-id="8dca3-131">string</span><span class="sxs-lookup"><span data-stu-id="8dca3-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="8dca3-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8dca3-132">Request body</span></span>
<span data-ttu-id="8dca3-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8dca3-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dca3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dca3-134">Response</span></span>

<span data-ttu-id="8dca3-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [onenoteSection](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8dca3-135">If successful, this method returns a `200 OK` response code and collection of [onenoteSection](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8dca3-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8dca3-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8dca3-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dca3-137">Request</span></span>
<span data-ttu-id="8dca3-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8dca3-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections
```
##### <a name="response"></a><span data-ttu-id="8dca3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dca3-139">Response</span></span>
<span data-ttu-id="8dca3-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8dca3-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->