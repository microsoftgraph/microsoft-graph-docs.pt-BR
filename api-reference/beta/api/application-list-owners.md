---
title: Listar proprietários
description: Recupere uma lista de proprietários (objetos directoryobject) para um aplicativo.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da9944bf44e7b5352c22a2e69e4e54da9a2aeb7c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289324"
---
# <a name="list-owners"></a><span data-ttu-id="90ee3-103">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="90ee3-103">List owners</span></span>

<span data-ttu-id="90ee3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90ee3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90ee3-105">Recupere uma lista de proprietários para um aplicativo que são objetos [directoryobject](../resources/directoryobject.md) .</span><span class="sxs-lookup"><span data-stu-id="90ee3-105">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="90ee3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="90ee3-106">Permissions</span></span>
<span data-ttu-id="90ee3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90ee3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90ee3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90ee3-109">Permission type</span></span>      | <span data-ttu-id="90ee3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90ee3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90ee3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90ee3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="90ee3-112">Application. Read. All, Directory. Read. All, Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="90ee3-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="90ee3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90ee3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90ee3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90ee3-114">Not supported.</span></span>    |
|<span data-ttu-id="90ee3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90ee3-115">Application</span></span> | <span data-ttu-id="90ee3-116">Application. Read. All, Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="90ee3-116">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="90ee3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90ee3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="90ee3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="90ee3-118">Optional query parameters</span></span>
<span data-ttu-id="90ee3-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="90ee3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90ee3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90ee3-120">Request headers</span></span>
| <span data-ttu-id="90ee3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="90ee3-121">Name</span></span>           | <span data-ttu-id="90ee3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="90ee3-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="90ee3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90ee3-123">Authorization</span></span>  | <span data-ttu-id="90ee3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90ee3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="90ee3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90ee3-126">Request body</span></span>
<span data-ttu-id="90ee3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90ee3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90ee3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ee3-128">Response</span></span>

<span data-ttu-id="90ee3-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90ee3-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="90ee3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90ee3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90ee3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90ee3-131">Request</span></span>
<span data-ttu-id="90ee3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90ee3-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90ee3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="90ee3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="90ee3-134">C#</span><span class="sxs-lookup"><span data-stu-id="90ee3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90ee3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90ee3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90ee3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90ee3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="90ee3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ee3-137">Response</span></span>
<span data-ttu-id="90ee3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90ee3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
