---
title: 'servicePrincipalName: listar createdObjects'
description: Recupere uma lista de objetos directoryobject.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 74d23f1fb682cb0c0e06c9d1260d7c478bbdfa43
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219078"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="00aed-103">servicePrincipalName: listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="00aed-103">servicePrincipal: List createdObjects</span></span>

<span data-ttu-id="00aed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00aed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00aed-105">Recupere uma lista de objetos directoryobject.</span><span class="sxs-lookup"><span data-stu-id="00aed-105">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="00aed-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="00aed-106">Permissions</span></span>
<span data-ttu-id="00aed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00aed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00aed-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00aed-109">Permission type</span></span>      | <span data-ttu-id="00aed-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00aed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00aed-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00aed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00aed-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="00aed-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="00aed-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00aed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00aed-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00aed-114">Not supported.</span></span>    |
|<span data-ttu-id="00aed-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00aed-115">Application</span></span> | <span data-ttu-id="00aed-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00aed-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="00aed-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00aed-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="00aed-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="00aed-118">Optional query parameters</span></span>
<span data-ttu-id="00aed-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="00aed-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00aed-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00aed-120">Request headers</span></span>
| <span data-ttu-id="00aed-121">Nome</span><span class="sxs-lookup"><span data-stu-id="00aed-121">Name</span></span>       | <span data-ttu-id="00aed-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="00aed-122">Type</span></span> | <span data-ttu-id="00aed-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="00aed-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="00aed-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="00aed-124">Authorization</span></span>  | <span data-ttu-id="00aed-125">string</span><span class="sxs-lookup"><span data-stu-id="00aed-125">string</span></span>  | <span data-ttu-id="00aed-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00aed-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00aed-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00aed-128">Request body</span></span>
<span data-ttu-id="00aed-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00aed-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00aed-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="00aed-130">Response</span></span>

<span data-ttu-id="00aed-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00aed-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00aed-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00aed-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00aed-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00aed-133">Request</span></span>
<span data-ttu-id="00aed-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00aed-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="00aed-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="00aed-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipals_get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="00aed-136">C#</span><span class="sxs-lookup"><span data-stu-id="00aed-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00aed-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00aed-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00aed-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00aed-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="00aed-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="00aed-139">Response</span></span>
<span data-ttu-id="00aed-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00aed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
