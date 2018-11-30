---
title: Listar blocos de anotações
description: Recupere uma lista de objetos notebook.
ms.openlocfilehash: 429c02d0032453fc00a7517af32cac8b9d3c66f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006234"
---
# <a name="list-notebooks"></a><span data-ttu-id="941e9-103">Listar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="941e9-103">List notebooks</span></span>

<span data-ttu-id="941e9-104">Recupere uma lista de objetos [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="941e9-104">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="941e9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="941e9-105">Permissions</span></span>
<span data-ttu-id="941e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="941e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="941e9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="941e9-108">Permission type</span></span>      | <span data-ttu-id="941e9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="941e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="941e9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="941e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="941e9-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941e9-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="941e9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="941e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="941e9-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="941e9-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="941e9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="941e9-114">Application</span></span> | <span data-ttu-id="941e9-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941e9-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="941e9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="941e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="941e9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="941e9-117">Optional query parameters</span></span>
<span data-ttu-id="941e9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="941e9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="941e9-119">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="941e9-119">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="941e9-120">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="941e9-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="941e9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="941e9-121">Request headers</span></span>
| <span data-ttu-id="941e9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="941e9-122">Name</span></span>       | <span data-ttu-id="941e9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="941e9-123">Type</span></span> | <span data-ttu-id="941e9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="941e9-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="941e9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="941e9-125">Authorization</span></span>  | <span data-ttu-id="941e9-126">string</span><span class="sxs-lookup"><span data-stu-id="941e9-126">string</span></span>  | <span data-ttu-id="941e9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="941e9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="941e9-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="941e9-129">Accept</span></span> | <span data-ttu-id="941e9-130">string</span><span class="sxs-lookup"><span data-stu-id="941e9-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="941e9-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="941e9-131">Request body</span></span>
<span data-ttu-id="941e9-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="941e9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="941e9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="941e9-133">Response</span></span>

<span data-ttu-id="941e9-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="941e9-134">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="941e9-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="941e9-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="941e9-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="941e9-136">Request</span></span>
<span data-ttu-id="941e9-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="941e9-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="941e9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="941e9-138">Response</span></span>
<span data-ttu-id="941e9-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="941e9-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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