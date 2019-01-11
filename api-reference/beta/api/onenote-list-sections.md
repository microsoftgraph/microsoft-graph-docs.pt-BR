---
title: Listar seções
description: Recupere uma lista de objetos section.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 11636dd2fbb0c39724b0036bdfa5db03bb12f0c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857691"
---
# <a name="list-sections"></a><span data-ttu-id="ae358-103">Listar seções</span><span class="sxs-lookup"><span data-stu-id="ae358-103">List sections</span></span>

> <span data-ttu-id="ae358-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ae358-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae358-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ae358-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae358-106">Recupere uma lista de objetos [section](../resources/section.md).</span><span class="sxs-lookup"><span data-stu-id="ae358-106">Retrieve a list of [section](../resources/section.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae358-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae358-107">Permissions</span></span>
<span data-ttu-id="ae358-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae358-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae358-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae358-110">Permission type</span></span>      | <span data-ttu-id="ae358-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae358-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae358-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae358-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ae358-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae358-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ae358-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae358-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae358-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae358-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ae358-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae358-116">Application</span></span> | <span data-ttu-id="ae358-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae358-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae358-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae358-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections
GET /users/{id | userPrincipalName}/onenote/sections
GET /groups/{id}/onenote/sections
GET /sites/{id}/onenote/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae358-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ae358-119">Optional query parameters</span></span>
<span data-ttu-id="ae358-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ae358-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ae358-121">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="ae358-121">The default sort order is `name asc`.</span></span>

<span data-ttu-id="ae358-p103">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="ae358-p103">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae358-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae358-124">Request headers</span></span>
| <span data-ttu-id="ae358-125">Nome</span><span class="sxs-lookup"><span data-stu-id="ae358-125">Name</span></span>       | <span data-ttu-id="ae358-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae358-126">Type</span></span> | <span data-ttu-id="ae358-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae358-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ae358-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae358-128">Authorization</span></span>  | <span data-ttu-id="ae358-129">string</span><span class="sxs-lookup"><span data-stu-id="ae358-129">string</span></span>  | <span data-ttu-id="ae358-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae358-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae358-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae358-132">Accept</span></span> | <span data-ttu-id="ae358-133">string</span><span class="sxs-lookup"><span data-stu-id="ae358-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ae358-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae358-134">Request body</span></span>
<span data-ttu-id="ae358-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae358-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae358-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae358-136">Response</span></span>

<span data-ttu-id="ae358-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [section](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae358-137">If successful, this method returns a `200 OK` response code and collection of [section](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae358-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae358-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae358-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae358-139">Request</span></span>
<span data-ttu-id="ae358-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae358-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections
```
##### <a name="response"></a><span data-ttu-id="ae358-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae358-141">Response</span></span>
<span data-ttu-id="ae358-p105">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae358-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
