---
title: Obter bloco de anotações
description: Recupere as propriedades e os relacionamentos de um objeto notebook.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: af8d358a7f05ed60b48e6df6a3cc60319e009e34
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540322"
---
# <a name="get-notebook"></a><span data-ttu-id="3ec25-103">Obter bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="3ec25-103">Get notebook</span></span>

<span data-ttu-id="3ec25-104">Recupere as propriedades e os relacionamentos de um objeto [Notebook](../resources/notebook.md) .</span><span class="sxs-lookup"><span data-stu-id="3ec25-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ec25-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ec25-105">Permissions</span></span>
<span data-ttu-id="3ec25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ec25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ec25-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ec25-108">Permission type</span></span>      | <span data-ttu-id="3ec25-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ec25-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ec25-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ec25-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ec25-111">Notes. Create, Notes. Read, Notes. ReadWrite, Notes. Read. All, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3ec25-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3ec25-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ec25-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ec25-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec25-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3ec25-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ec25-114">Application</span></span> | <span data-ttu-id="3ec25-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec25-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ec25-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec25-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3ec25-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3ec25-117">Optional query parameters</span></span>
<span data-ttu-id="3ec25-118">Este método oferece suporte `select` aos `expand` [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3ec25-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="3ec25-119">Os `expand` valores válidos para blocos de `sections` anotações `sectionGroups`são e.</span><span class="sxs-lookup"><span data-stu-id="3ec25-119">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ec25-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ec25-120">Request headers</span></span>
| <span data-ttu-id="3ec25-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3ec25-121">Name</span></span>       | <span data-ttu-id="3ec25-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ec25-122">Type</span></span> | <span data-ttu-id="3ec25-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ec25-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3ec25-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ec25-124">Authorization</span></span>  | <span data-ttu-id="3ec25-125">string</span><span class="sxs-lookup"><span data-stu-id="3ec25-125">string</span></span>  | <span data-ttu-id="3ec25-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ec25-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ec25-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3ec25-128">Accept</span></span> | <span data-ttu-id="3ec25-129">string</span><span class="sxs-lookup"><span data-stu-id="3ec25-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3ec25-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ec25-130">Request body</span></span>
<span data-ttu-id="3ec25-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ec25-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ec25-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ec25-132">Response</span></span>

<span data-ttu-id="3ec25-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ec25-133">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3ec25-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ec25-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ec25-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ec25-135">Request</span></span>
<span data-ttu-id="3ec25-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ec25-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="3ec25-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ec25-137">Response</span></span>
<span data-ttu-id="3ec25-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ec25-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
