---
title: List servicePrincipals
description: Recupere uma lista de objetos servicePrincipal.
localization_priority: Normal
ms.openlocfilehash: 4b408e0af724c6a4b406ca30aef5c77ace50325e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263774"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="eb0e6-103">List servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="eb0e6-103">List servicePrincipals</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb0e6-104">Recupere uma lista de objetos servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-104">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb0e6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb0e6-105">Permissions</span></span>

<span data-ttu-id="eb0e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb0e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eb0e6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb0e6-108">Permission type</span></span>      | <span data-ttu-id="eb0e6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb0e6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb0e6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb0e6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eb0e6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eb0e6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eb0e6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb0e6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb0e6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-113">Not supported.</span></span>    |
|<span data-ttu-id="eb0e6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb0e6-114">Application</span></span> | <span data-ttu-id="eb0e6-115">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb0e6-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb0e6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb0e6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eb0e6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eb0e6-117">Optional query parameters</span></span>

<span data-ttu-id="eb0e6-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb0e6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb0e6-119">Request headers</span></span>
| <span data-ttu-id="eb0e6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="eb0e6-120">Name</span></span> | <span data-ttu-id="eb0e6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb0e6-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="eb0e6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb0e6-122">Authorization</span></span>  | <span data-ttu-id="eb0e6-123">string</span><span class="sxs-lookup"><span data-stu-id="eb0e6-123">string</span></span>  | <span data-ttu-id="eb0e6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb0e6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb0e6-126">Request body</span></span>

<span data-ttu-id="eb0e6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb0e6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb0e6-128">Response</span></span>

<span data-ttu-id="eb0e6-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos de [servicePrincipalName](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb0e6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb0e6-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eb0e6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb0e6-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
##### <a name="response"></a><span data-ttu-id="eb0e6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb0e6-132">Response</span></span>

<span data-ttu-id="eb0e6-p103">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb0e6-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 488

{
  "value": [
    {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="eb0e6-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="eb0e6-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eb0e6-136">C#</span><span class="sxs-lookup"><span data-stu-id="eb0e6-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_serviceprincipals-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb0e6-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb0e6-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_serviceprincipals-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="eb0e6-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="eb0e6-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_serviceprincipals-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/serviceprincipal-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
