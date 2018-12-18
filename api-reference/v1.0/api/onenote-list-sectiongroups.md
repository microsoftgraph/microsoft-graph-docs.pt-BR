---
title: Listar sectionGroups
description: Recupere uma lista de objetossectionGroup.
author: Jewan-microsoft
ms.openlocfilehash: 3f33f8b7b35cb5b1d4408b0a8f2ec6e4c968bfc9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341494"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="1dfe6-103">Listar sectionGroups</span><span class="sxs-lookup"><span data-stu-id="1dfe6-103">List sectionGroups</span></span>

<span data-ttu-id="1dfe6-104">Recupere uma lista de objetos[sectionGroup](../resources/sectiongroup.md).</span><span class="sxs-lookup"><span data-stu-id="1dfe6-104">Retrieve a list of [sectionGroup](../resources/sectiongroup.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1dfe6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1dfe6-105">Permissions</span></span>
<span data-ttu-id="1dfe6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dfe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dfe6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dfe6-108">Permission type</span></span>      | <span data-ttu-id="1dfe6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1dfe6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dfe6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dfe6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1dfe6-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dfe6-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1dfe6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dfe6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dfe6-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1dfe6-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1dfe6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfe6-114">Application</span></span> | <span data-ttu-id="1dfe6-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dfe6-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dfe6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dfe6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups
GET /groups/{id}/onenote/sectionGroups
GET /sites/{id}/onenote/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1dfe6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1dfe6-117">Optional query parameters</span></span>
<span data-ttu-id="1dfe6-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1dfe6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1dfe6-119">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="1dfe6-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="1dfe6-p102">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `sections`, `sectionGroups`, `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="1dfe6-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1dfe6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dfe6-122">Request headers</span></span>
| <span data-ttu-id="1dfe6-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1dfe6-123">Name</span></span>       | <span data-ttu-id="1dfe6-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dfe6-124">Type</span></span> | <span data-ttu-id="1dfe6-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dfe6-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1dfe6-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dfe6-126">Authorization</span></span>  | <span data-ttu-id="1dfe6-127">string</span><span class="sxs-lookup"><span data-stu-id="1dfe6-127">string</span></span>  | <span data-ttu-id="1dfe6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dfe6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1dfe6-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1dfe6-130">Accept</span></span> | <span data-ttu-id="1dfe6-131">string</span><span class="sxs-lookup"><span data-stu-id="1dfe6-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1dfe6-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dfe6-132">Request body</span></span>
<span data-ttu-id="1dfe6-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1dfe6-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dfe6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dfe6-134">Response</span></span>

<span data-ttu-id="1dfe6-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1dfe6-135">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1dfe6-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dfe6-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1dfe6-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dfe6-137">Request</span></span>
<span data-ttu-id="1dfe6-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dfe6-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="1dfe6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dfe6-139">Response</span></span>
<span data-ttu-id="1dfe6-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1dfe6-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 378

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->