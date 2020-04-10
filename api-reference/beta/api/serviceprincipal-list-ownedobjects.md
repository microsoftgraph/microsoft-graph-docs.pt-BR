---
title: 'servicePrincipalName: listar ownedObjects'
description: Recupere uma lista de objetos pertencentes ao servicePrincipalName.  Isso pode incluir aplicativos ou grupos.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 52ad61baddd38e49bc57755daadb8553823ac2ca
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219050"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="42e6f-104">servicePrincipalName: listar ownedObjects</span><span class="sxs-lookup"><span data-stu-id="42e6f-104">servicePrincipals: List ownedObjects</span></span>

<span data-ttu-id="42e6f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42e6f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42e6f-106">Recupere uma lista de objetos pertencentes ao servicePrincipalName.</span><span class="sxs-lookup"><span data-stu-id="42e6f-106">Retrieve a list of objects owned by the servicePrincipal.</span></span>  <span data-ttu-id="42e6f-107">Isso pode incluir aplicativos ou grupos.</span><span class="sxs-lookup"><span data-stu-id="42e6f-107">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="42e6f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="42e6f-108">Permissions</span></span>
<span data-ttu-id="42e6f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42e6f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42e6f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42e6f-111">Permission type</span></span>      | <span data-ttu-id="42e6f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42e6f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42e6f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42e6f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="42e6f-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="42e6f-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="42e6f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42e6f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42e6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42e6f-116">Not supported.</span></span>    |
|<span data-ttu-id="42e6f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42e6f-117">Application</span></span> | <span data-ttu-id="42e6f-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42e6f-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="42e6f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42e6f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="42e6f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="42e6f-120">Optional query parameters</span></span>
<span data-ttu-id="42e6f-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="42e6f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42e6f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42e6f-122">Request headers</span></span>
| <span data-ttu-id="42e6f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="42e6f-123">Name</span></span>       | <span data-ttu-id="42e6f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="42e6f-124">Type</span></span> | <span data-ttu-id="42e6f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="42e6f-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="42e6f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="42e6f-126">Authorization</span></span>  | <span data-ttu-id="42e6f-127">string</span><span class="sxs-lookup"><span data-stu-id="42e6f-127">string</span></span>  | <span data-ttu-id="42e6f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42e6f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42e6f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42e6f-130">Request body</span></span>
<span data-ttu-id="42e6f-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42e6f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42e6f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="42e6f-132">Response</span></span>

<span data-ttu-id="42e6f-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42e6f-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42e6f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42e6f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42e6f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42e6f-135">Request</span></span>
<span data-ttu-id="42e6f-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42e6f-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42e6f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="42e6f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="42e6f-138">C#</span><span class="sxs-lookup"><span data-stu-id="42e6f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42e6f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42e6f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42e6f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42e6f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="42e6f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="42e6f-141">Response</span></span>
<span data-ttu-id="42e6f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42e6f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
