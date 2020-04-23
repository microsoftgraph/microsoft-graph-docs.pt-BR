---
title: Listar o servicePrincipalName memberOf
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro direto. Essa operação não é transitiva.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 50b5e26d9deb461ac672b7529450e092055824fd
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219064"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="11a42-104">Listar o servicePrincipalName memberOf</span><span class="sxs-lookup"><span data-stu-id="11a42-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="11a42-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11a42-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11a42-106">Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro direto.</span><span class="sxs-lookup"><span data-stu-id="11a42-106">Get the groups and directory roles that this service principal is a direct member of.</span></span> <span data-ttu-id="11a42-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="11a42-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="11a42-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="11a42-108">Permissions</span></span>

<span data-ttu-id="11a42-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11a42-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11a42-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11a42-111">Permission type</span></span>      | <span data-ttu-id="11a42-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11a42-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11a42-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11a42-113">Delegated (work or school account)</span></span> | <span data-ttu-id="11a42-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="11a42-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="11a42-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11a42-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11a42-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11a42-116">Not supported.</span></span>    |
|<span data-ttu-id="11a42-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11a42-117">Application</span></span> | <span data-ttu-id="11a42-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11a42-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="11a42-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11a42-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="11a42-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="11a42-120">Optional query parameters</span></span>

<span data-ttu-id="11a42-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="11a42-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11a42-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11a42-122">Request headers</span></span>
| <span data-ttu-id="11a42-123">Nome</span><span class="sxs-lookup"><span data-stu-id="11a42-123">Name</span></span>       | <span data-ttu-id="11a42-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="11a42-124">Type</span></span> | <span data-ttu-id="11a42-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="11a42-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="11a42-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="11a42-126">Authorization</span></span>  | <span data-ttu-id="11a42-127">string</span><span class="sxs-lookup"><span data-stu-id="11a42-127">string</span></span>  | <span data-ttu-id="11a42-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11a42-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11a42-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11a42-130">Request body</span></span>
<span data-ttu-id="11a42-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11a42-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11a42-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="11a42-132">Response</span></span>

<span data-ttu-id="11a42-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11a42-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11a42-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11a42-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="11a42-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11a42-135">Request</span></span>

<span data-ttu-id="11a42-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11a42-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11a42-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="11a42-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="11a42-138">C#</span><span class="sxs-lookup"><span data-stu-id="11a42-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11a42-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11a42-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11a42-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11a42-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11a42-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="11a42-141">Response</span></span>

<span data-ttu-id="11a42-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11a42-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
