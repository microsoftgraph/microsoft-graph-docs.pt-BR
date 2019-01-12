---
title: Obter sectionGroup
description: Recupere as propriedades e os relacionamentos de um objeto sectionGroup.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 81b838d01517d219fdb3375140092bf44f58f793
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953291"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="d0984-103">Obter sectionGroup</span><span class="sxs-lookup"><span data-stu-id="d0984-103">Get sectionGroup</span></span>

> <span data-ttu-id="d0984-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d0984-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0984-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d0984-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0984-106">Recupere as propriedades e os relacionamentos de um objeto [sectionGroup](../resources/sectiongroup.md).</span><span class="sxs-lookup"><span data-stu-id="d0984-106">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d0984-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0984-107">Permissions</span></span>
<span data-ttu-id="d0984-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0984-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0984-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0984-110">Permission type</span></span>      | <span data-ttu-id="d0984-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0984-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0984-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0984-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0984-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0984-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0984-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0984-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0984-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0984-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d0984-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0984-116">Application</span></span> | <span data-ttu-id="d0984-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0984-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0984-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0984-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d0984-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d0984-119">Optional query parameters</span></span>
<span data-ttu-id="d0984-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d0984-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d0984-p103">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `name` e `self`. Os valores `expand` válidos para o grupo de seção são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="d0984-p103">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties. Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0984-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0984-123">Request headers</span></span>
| <span data-ttu-id="d0984-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d0984-124">Name</span></span>       | <span data-ttu-id="d0984-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0984-125">Type</span></span> | <span data-ttu-id="d0984-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0984-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d0984-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0984-127">Authorization</span></span>  | <span data-ttu-id="d0984-128">string</span><span class="sxs-lookup"><span data-stu-id="d0984-128">string</span></span>  | <span data-ttu-id="d0984-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0984-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0984-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0984-131">Accept</span></span> | <span data-ttu-id="d0984-132">string</span><span class="sxs-lookup"><span data-stu-id="d0984-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d0984-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0984-133">Request body</span></span>
<span data-ttu-id="d0984-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0984-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0984-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0984-135">Response</span></span>

<span data-ttu-id="d0984-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0984-136">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0984-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0984-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0984-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0984-138">Request</span></span>
<span data-ttu-id="d0984-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0984-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="d0984-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0984-140">Response</span></span>
<span data-ttu-id="d0984-p105">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0984-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
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
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
