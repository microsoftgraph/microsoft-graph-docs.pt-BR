---
title: Listar blocos de anotações
description: Recuperar uma lista de objetos do bloco de anotações.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: c0de11f9c42f6204660f57dfb78f601eb612b73f
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473917"
---
# <a name="list-notebooks"></a><span data-ttu-id="477b4-103">Listar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="477b4-103">List notebooks</span></span>

<span data-ttu-id="477b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="477b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="477b4-105">Recupere uma lista de objetos [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="477b4-105">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="477b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="477b4-106">Permissions</span></span>
<span data-ttu-id="477b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="477b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="477b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="477b4-109">Permission type</span></span>      | <span data-ttu-id="477b4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="477b4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="477b4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="477b4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="477b4-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="477b4-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="477b4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="477b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="477b4-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="477b4-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="477b4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="477b4-115">Application</span></span> | <span data-ttu-id="477b4-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="477b4-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="477b4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="477b4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="477b4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="477b4-118">Optional query parameters</span></span>
<span data-ttu-id="477b4-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="477b4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="477b4-120">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="477b4-120">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="477b4-121">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="477b4-121">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="477b4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="477b4-122">Request headers</span></span>
| <span data-ttu-id="477b4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="477b4-123">Name</span></span>       | <span data-ttu-id="477b4-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="477b4-124">Type</span></span> | <span data-ttu-id="477b4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="477b4-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="477b4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="477b4-126">Authorization</span></span>  | <span data-ttu-id="477b4-127">string</span><span class="sxs-lookup"><span data-stu-id="477b4-127">string</span></span>  | <span data-ttu-id="477b4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="477b4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="477b4-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="477b4-130">Accept</span></span> | <span data-ttu-id="477b4-131">string</span><span class="sxs-lookup"><span data-stu-id="477b4-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="477b4-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="477b4-132">Request body</span></span>
<span data-ttu-id="477b4-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="477b4-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="477b4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="477b4-134">Response</span></span>

<span data-ttu-id="477b4-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="477b4-135">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="477b4-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="477b4-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="477b4-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="477b4-137">Request</span></span>
<span data-ttu-id="477b4-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="477b4-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="477b4-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="477b4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
# <a name="c"></a>[<span data-ttu-id="477b4-140">C#</span><span class="sxs-lookup"><span data-stu-id="477b4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebooks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="477b4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="477b4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebooks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="477b4-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="477b4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebooks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="477b4-143">Java</span><span class="sxs-lookup"><span data-stu-id="477b4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-notebooks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="477b4-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="477b4-144">Response</span></span>
<span data-ttu-id="477b4-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="477b4-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "isDefault": true,
      "userRole":  "Owner",
      "isShared": false,
      "sectionsUrl": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d/sections",
      "sectionGroupsUrl": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d/sectionGroups",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
      "links": {
        "oneNoteClientUrl": {
          "href": "onenote:https://contoso-my.sharepoint.com/personal/admin_m365x841051_onmicrosoft_com/Documents/Notebooks/My%20Private%20notebook"
        },
        "oneNoteWebUrl": {
          "href": "https://contoso-my.sharepoint.com/personal/admin_m365x841051_onmicrosoft_com/Documents/Notebooks/My%20Private%20notebook"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
