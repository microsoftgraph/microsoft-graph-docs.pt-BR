---
title: 'servicePrincipalName: listar createdObjects'
description: Recupere uma lista de objetos directoryobject.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 7f4ebd1229a702cbb77e6b13aeeef0be9c118b30
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044575"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="47629-103">servicePrincipalName: listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="47629-103">servicePrincipal: List createdObjects</span></span>

<span data-ttu-id="47629-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47629-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47629-105">Recupere uma lista de objetos directoryobject.</span><span class="sxs-lookup"><span data-stu-id="47629-105">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="47629-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="47629-106">Permissions</span></span>
<span data-ttu-id="47629-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47629-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47629-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47629-109">Permission type</span></span>      | <span data-ttu-id="47629-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47629-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47629-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47629-111">Delegated (work or school account)</span></span> | <span data-ttu-id="47629-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="47629-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="47629-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47629-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47629-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47629-114">Not supported.</span></span>    |
|<span data-ttu-id="47629-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47629-115">Application</span></span> | <span data-ttu-id="47629-116">Application. Read. All, Directory. Read. All, Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="47629-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="47629-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47629-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="47629-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47629-118">Optional query parameters</span></span>
<span data-ttu-id="47629-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="47629-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47629-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47629-120">Request headers</span></span>
| <span data-ttu-id="47629-121">Nome</span><span class="sxs-lookup"><span data-stu-id="47629-121">Name</span></span>           | <span data-ttu-id="47629-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="47629-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="47629-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="47629-123">Authorization</span></span>  | <span data-ttu-id="47629-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47629-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47629-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47629-126">Request body</span></span>
<span data-ttu-id="47629-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47629-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47629-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="47629-128">Response</span></span>

<span data-ttu-id="47629-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47629-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="47629-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47629-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="47629-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47629-131">Request</span></span>
<span data-ttu-id="47629-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47629-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="47629-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="47629-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipals_get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="47629-134">C#</span><span class="sxs-lookup"><span data-stu-id="47629-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47629-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47629-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47629-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47629-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="47629-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="47629-137">Response</span></span>
<span data-ttu-id="47629-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47629-138">Here is an example of the response.</span></span> 
><span data-ttu-id="47629-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47629-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


