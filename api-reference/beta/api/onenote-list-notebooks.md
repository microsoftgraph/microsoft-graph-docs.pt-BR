---
title: Listar blocos de anotações
description: Recuperar uma lista de objetos do bloco de anotações.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 7cb6ac9d453726a8cd1b743d2fad5eb2fc4b57c0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981269"
---
# <a name="list-notebooks"></a><span data-ttu-id="04db4-103">Listar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="04db4-103">List notebooks</span></span>

<span data-ttu-id="04db4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04db4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04db4-105">Recupere uma lista de objetos [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="04db4-105">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="04db4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="04db4-106">Permissions</span></span>
<span data-ttu-id="04db4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04db4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04db4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04db4-109">Permission type</span></span>      | <span data-ttu-id="04db4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04db4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04db4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04db4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="04db4-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04db4-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="04db4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04db4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04db4-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04db4-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="04db4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04db4-115">Application</span></span> | <span data-ttu-id="04db4-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04db4-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04db4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04db4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="04db4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="04db4-118">Optional query parameters</span></span>
<span data-ttu-id="04db4-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="04db4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="04db4-120">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="04db4-120">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="04db4-121">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="04db4-121">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04db4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04db4-122">Request headers</span></span>
| <span data-ttu-id="04db4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="04db4-123">Name</span></span>       | <span data-ttu-id="04db4-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="04db4-124">Type</span></span> | <span data-ttu-id="04db4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="04db4-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="04db4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="04db4-126">Authorization</span></span>  | <span data-ttu-id="04db4-127">string</span><span class="sxs-lookup"><span data-stu-id="04db4-127">string</span></span>  | <span data-ttu-id="04db4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04db4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04db4-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04db4-130">Accept</span></span> | <span data-ttu-id="04db4-131">string</span><span class="sxs-lookup"><span data-stu-id="04db4-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="04db4-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04db4-132">Request body</span></span>
<span data-ttu-id="04db4-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04db4-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04db4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="04db4-134">Response</span></span>

<span data-ttu-id="04db4-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04db4-135">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04db4-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04db4-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04db4-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04db4-137">Request</span></span>
<span data-ttu-id="04db4-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04db4-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04db4-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="04db4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
# <a name="c"></a>[<span data-ttu-id="04db4-140">C#</span><span class="sxs-lookup"><span data-stu-id="04db4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebooks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04db4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04db4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebooks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04db4-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04db4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebooks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04db4-143">Java</span><span class="sxs-lookup"><span data-stu-id="04db4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-notebooks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="04db4-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="04db4-144">Response</span></span>
<span data-ttu-id="04db4-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04db4-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
