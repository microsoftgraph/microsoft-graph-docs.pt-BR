---
title: Listar os memberOf transitivos de servicePrincipalName
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro. Essa operação é transitiva e inclui todos os grupos dos quais essa entidade de serviço é um membro aninhado.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 519afa4f7a4e3477250641a5d1fc109404f6db6e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867831"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="0b234-104">Listar os memberOf transitivos de servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="0b234-104">List servicePrincipal transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b234-105">Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro.</span><span class="sxs-lookup"><span data-stu-id="0b234-105">Get the groups and directory roles that this service principal is a member of.</span></span> <span data-ttu-id="0b234-106">Essa operação é transitiva e inclui todos os grupos dos quais essa entidade de serviço é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="0b234-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b234-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b234-107">Permissions</span></span>
<span data-ttu-id="0b234-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b234-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b234-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b234-110">Permission type</span></span>      | <span data-ttu-id="0b234-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b234-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b234-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b234-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0b234-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b234-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0b234-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b234-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b234-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b234-115">Not supported.</span></span>    |
|<span data-ttu-id="0b234-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b234-116">Application</span></span> | <span data-ttu-id="0b234-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b234-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0b234-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b234-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0b234-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0b234-119">Optional query parameters</span></span>
<span data-ttu-id="0b234-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0b234-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b234-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b234-121">Request headers</span></span>
| <span data-ttu-id="0b234-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0b234-122">Name</span></span>       | <span data-ttu-id="0b234-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b234-123">Type</span></span> | <span data-ttu-id="0b234-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b234-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0b234-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b234-125">Authorization</span></span>  | <span data-ttu-id="0b234-126">string</span><span class="sxs-lookup"><span data-stu-id="0b234-126">string</span></span>  | <span data-ttu-id="0b234-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b234-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b234-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b234-129">Request body</span></span>
<span data-ttu-id="0b234-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b234-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b234-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b234-131">Response</span></span>

<span data-ttu-id="0b234-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b234-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b234-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b234-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b234-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b234-134">Request</span></span>

<span data-ttu-id="0b234-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b234-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b234-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b234-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b234-137">C#</span><span class="sxs-lookup"><span data-stu-id="0b234-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b234-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b234-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b234-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b234-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b234-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b234-140">Response</span></span>

<span data-ttu-id="0b234-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b234-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
