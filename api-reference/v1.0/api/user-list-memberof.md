---
title: Listar memberOf
description: 'Obtenha todos os grupos e funções de diretório dos quais o usuário é um membro direto. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 82980451bb30ef954399812a628b170445f2819d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273014"
---
# <a name="list-memberof"></a><span data-ttu-id="6d2a3-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="6d2a3-103">List memberOf</span></span>

<span data-ttu-id="6d2a3-104">Obtenha [grupos](../resources/group.md) e [funções de diretório](../resources/directoryrole.md) dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="6d2a3-104">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6d2a3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d2a3-105">Permissions</span></span>
<span data-ttu-id="6d2a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d2a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d2a3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d2a3-108">Permission type</span></span>      | <span data-ttu-id="6d2a3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d2a3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d2a3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d2a3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6d2a3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6d2a3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6d2a3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d2a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d2a3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d2a3-113">Not supported.</span></span>    |
|<span data-ttu-id="6d2a3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d2a3-114">Application</span></span> | <span data-ttu-id="6d2a3-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d2a3-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d2a3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d2a3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6d2a3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6d2a3-117">Optional query parameters</span></span>
<span data-ttu-id="6d2a3-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6d2a3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="6d2a3-119">$filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="6d2a3-119">$filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="6d2a3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d2a3-120">Request headers</span></span>
| <span data-ttu-id="6d2a3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d2a3-121">Header</span></span>       | <span data-ttu-id="6d2a3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6d2a3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6d2a3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d2a3-123">Authorization</span></span>  | <span data-ttu-id="6d2a3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d2a3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6d2a3-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d2a3-126">Accept</span></span>  | <span data-ttu-id="6d2a3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6d2a3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d2a3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d2a3-128">Request body</span></span>
<span data-ttu-id="6d2a3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d2a3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d2a3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d2a3-130">Response</span></span>

<span data-ttu-id="6d2a3-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d2a3-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6d2a3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d2a3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d2a3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d2a3-133">Request</span></span>
<span data-ttu-id="6d2a3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d2a3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
##### <a name="response"></a><span data-ttu-id="6d2a3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d2a3-135">Response</span></span>
<span data-ttu-id="6d2a3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d2a3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6d2a3-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6d2a3-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6d2a3-140">C#</span><span class="sxs-lookup"><span data-stu-id="6d2a3-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_memberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d2a3-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="6d2a3-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_memberof-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6d2a3-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d2a3-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_memberof-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-memberof.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-list-memberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-memberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
