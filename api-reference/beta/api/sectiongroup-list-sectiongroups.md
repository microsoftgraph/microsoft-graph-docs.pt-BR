---
title: Listar sectionGroups
description: Recupere uma lista de objetos section groups do grupo de seção especificado.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 821898019737cd5fcd357acf4face5bbc83d4ea9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990527"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="1eb4a-103">Listar sectionGroups</span><span class="sxs-lookup"><span data-stu-id="1eb4a-103">List sectionGroups</span></span>

> <span data-ttu-id="1eb4a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1eb4a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1eb4a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1eb4a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1eb4a-106">Recupere uma lista de objetos [section groups](../resources/sectiongroup.md) do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="1eb4a-106">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="1eb4a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1eb4a-107">Permissions</span></span>
<span data-ttu-id="1eb4a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1eb4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1eb4a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1eb4a-110">Permission type</span></span>      | <span data-ttu-id="1eb4a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1eb4a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1eb4a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1eb4a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1eb4a-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eb4a-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1eb4a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1eb4a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1eb4a-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1eb4a-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1eb4a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1eb4a-116">Application</span></span> | <span data-ttu-id="1eb4a-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eb4a-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1eb4a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1eb4a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
GET /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
GET /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1eb4a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1eb4a-119">Optional query parameters</span></span>
<span data-ttu-id="1eb4a-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb4a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1eb4a-121">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="1eb4a-121">The default sort order is `name asc`.</span></span>

<span data-ttu-id="1eb4a-p103">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `sections`, `sectionGroups`, `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="1eb4a-p103">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1eb4a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb4a-124">Request headers</span></span>
| <span data-ttu-id="1eb4a-125">Nome</span><span class="sxs-lookup"><span data-stu-id="1eb4a-125">Name</span></span>       | <span data-ttu-id="1eb4a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="1eb4a-126">Type</span></span> | <span data-ttu-id="1eb4a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="1eb4a-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1eb4a-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="1eb4a-128">Authorization</span></span>  | <span data-ttu-id="1eb4a-129">string</span><span class="sxs-lookup"><span data-stu-id="1eb4a-129">string</span></span>  | <span data-ttu-id="1eb4a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1eb4a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1eb4a-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1eb4a-132">Accept</span></span> | <span data-ttu-id="1eb4a-133">string</span><span class="sxs-lookup"><span data-stu-id="1eb4a-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1eb4a-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb4a-134">Request body</span></span>
<span data-ttu-id="1eb4a-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1eb4a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1eb4a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb4a-136">Response</span></span>

<span data-ttu-id="1eb4a-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb4a-137">If successful, this method returns a `200 OK` response code and a collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1eb4a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1eb4a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1eb4a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb4a-139">Request</span></span>
<span data-ttu-id="1eb4a-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1eb4a-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="1eb4a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb4a-141">Response</span></span>
<span data-ttu-id="1eb4a-p105">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1eb4a-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup",
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
