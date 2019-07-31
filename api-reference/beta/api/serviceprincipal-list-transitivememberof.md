---
title: Listar os memberOf transitivos de servicePrincipalName
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro. Essa operação é transitiva e inclui todos os grupos dos quais essa entidade de serviço é um membro aninhado.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f4560b030debfdd9325733cc99210c4e9c436128
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977920"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="470be-104">Listar os memberOf transitivos de servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="470be-104">List servicePrincipal transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="470be-105">Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro.</span><span class="sxs-lookup"><span data-stu-id="470be-105">Get the groups and directory roles that this service principal is a member of.</span></span> <span data-ttu-id="470be-106">Essa operação é transitiva e inclui todos os grupos dos quais essa entidade de serviço é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="470be-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="470be-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="470be-107">Permissions</span></span>
<span data-ttu-id="470be-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="470be-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="470be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="470be-110">Permission type</span></span>      | <span data-ttu-id="470be-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="470be-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="470be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="470be-112">Delegated (work or school account)</span></span> | <span data-ttu-id="470be-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="470be-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="470be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="470be-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="470be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="470be-115">Not supported.</span></span>    |
|<span data-ttu-id="470be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="470be-116">Application</span></span> | <span data-ttu-id="470be-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="470be-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="470be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="470be-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="470be-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="470be-119">Optional query parameters</span></span>
<span data-ttu-id="470be-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="470be-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="470be-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="470be-121">Request headers</span></span>
| <span data-ttu-id="470be-122">Nome</span><span class="sxs-lookup"><span data-stu-id="470be-122">Name</span></span>       | <span data-ttu-id="470be-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="470be-123">Type</span></span> | <span data-ttu-id="470be-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="470be-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="470be-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="470be-125">Authorization</span></span>  | <span data-ttu-id="470be-126">string</span><span class="sxs-lookup"><span data-stu-id="470be-126">string</span></span>  | <span data-ttu-id="470be-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="470be-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="470be-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="470be-129">Request body</span></span>
<span data-ttu-id="470be-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="470be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="470be-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="470be-131">Response</span></span>

<span data-ttu-id="470be-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="470be-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="470be-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="470be-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="470be-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="470be-134">Request</span></span>

<span data-ttu-id="470be-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="470be-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="470be-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="470be-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="470be-137">C#</span><span class="sxs-lookup"><span data-stu-id="470be-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="470be-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="470be-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="470be-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="470be-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="470be-140">Java</span><span class="sxs-lookup"><span data-stu-id="470be-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="470be-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="470be-141">Response</span></span>

<span data-ttu-id="470be-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="470be-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
