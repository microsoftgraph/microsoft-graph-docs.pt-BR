---
title: Obter bloco de anotações
description: Recupere as propriedades e os relacionamentos de um objeto notebook.
author: Jewan-microsoft
ms.openlocfilehash: 1c4ef1db34f115e3904ff48b871e52f969b08d5a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334080"
---
# <a name="get-notebook"></a><span data-ttu-id="445f4-103">Obter bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="445f4-103">Get notebook</span></span>

> <span data-ttu-id="445f4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="445f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="445f4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="445f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="445f4-106">Recupere as propriedades e os relacionamentos de um objeto [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="445f4-106">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="445f4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="445f4-107">Permissions</span></span>
<span data-ttu-id="445f4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="445f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="445f4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="445f4-110">Permission type</span></span>      | <span data-ttu-id="445f4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="445f4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="445f4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="445f4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="445f4-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="445f4-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="445f4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="445f4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="445f4-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="445f4-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="445f4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="445f4-116">Application</span></span> | <span data-ttu-id="445f4-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="445f4-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="445f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="445f4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="445f4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="445f4-119">Optional query parameters</span></span>
<span data-ttu-id="445f4-120">Este método dá suporte a `select` e `expand` [Parâmetros de Consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="445f4-120">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="445f4-121">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="445f4-121">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="445f4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="445f4-122">Request headers</span></span>
| <span data-ttu-id="445f4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="445f4-123">Name</span></span>       | <span data-ttu-id="445f4-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="445f4-124">Type</span></span> | <span data-ttu-id="445f4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="445f4-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="445f4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="445f4-126">Authorization</span></span>  | <span data-ttu-id="445f4-127">string</span><span class="sxs-lookup"><span data-stu-id="445f4-127">string</span></span>  | <span data-ttu-id="445f4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="445f4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="445f4-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="445f4-130">Accept</span></span> | <span data-ttu-id="445f4-131">string</span><span class="sxs-lookup"><span data-stu-id="445f4-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="445f4-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="445f4-132">Request body</span></span>
<span data-ttu-id="445f4-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="445f4-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="445f4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="445f4-134">Response</span></span>

<span data-ttu-id="445f4-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="445f4-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="445f4-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="445f4-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="445f4-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="445f4-137">Request</span></span>
<span data-ttu-id="445f4-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="445f4-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="445f4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="445f4-139">Response</span></span>
<span data-ttu-id="445f4-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="445f4-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
