---
title: Listar blocos de anotações
description: Recupere uma lista de objetos notebook.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: f20d8c0002ca67a74f6008034ea25300b8aee5e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831091"
---
# <a name="list-notebooks"></a><span data-ttu-id="b165d-103">Listar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="b165d-103">List notebooks</span></span>

> <span data-ttu-id="b165d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b165d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b165d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b165d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b165d-106">Recupere uma lista de objetos [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="b165d-106">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b165d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b165d-107">Permissions</span></span>
<span data-ttu-id="b165d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b165d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b165d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b165d-110">Permission type</span></span>      | <span data-ttu-id="b165d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b165d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b165d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b165d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b165d-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b165d-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b165d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b165d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b165d-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b165d-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b165d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b165d-116">Application</span></span> | <span data-ttu-id="b165d-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b165d-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b165d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b165d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b165d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b165d-119">Optional query parameters</span></span>
<span data-ttu-id="b165d-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b165d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b165d-121">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="b165d-121">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="b165d-122">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="b165d-122">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b165d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b165d-123">Request headers</span></span>
| <span data-ttu-id="b165d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="b165d-124">Name</span></span>       | <span data-ttu-id="b165d-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="b165d-125">Type</span></span> | <span data-ttu-id="b165d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="b165d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b165d-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="b165d-127">Authorization</span></span>  | <span data-ttu-id="b165d-128">string</span><span class="sxs-lookup"><span data-stu-id="b165d-128">string</span></span>  | <span data-ttu-id="b165d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b165d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b165d-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b165d-131">Accept</span></span> | <span data-ttu-id="b165d-132">string</span><span class="sxs-lookup"><span data-stu-id="b165d-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b165d-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b165d-133">Request body</span></span>
<span data-ttu-id="b165d-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b165d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b165d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b165d-135">Response</span></span>

<span data-ttu-id="b165d-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b165d-136">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b165d-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b165d-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b165d-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b165d-138">Request</span></span>
<span data-ttu-id="b165d-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b165d-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="b165d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b165d-140">Response</span></span>
<span data-ttu-id="b165d-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b165d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
    {
      "isDefault": true,
      "userRole": {
      },
      "isShared": true,
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
      "links": {
        "oneNoteClientUrl": {
          "href": "href-value"
        },
        "oneNoteWebUrl": {
          "href": "href-value"
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
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
