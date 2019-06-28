---
title: Obter um servicePrincipal
description: Recuperar as propriedades e as relações do objeto serviceprincipal.
localization_priority: Priority
ms.openlocfilehash: 1e608d402adc59266050ba937b4462ff5637c3bf
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266924"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="95eb9-103">Obter um servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="95eb9-103">Get servicePrincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95eb9-104">Recuperar as propriedades e as relações do objeto serviceprincipal.</span><span class="sxs-lookup"><span data-stu-id="95eb9-104">Retrieve the properties and relationships of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="95eb9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="95eb9-105">Permissions</span></span>
<span data-ttu-id="95eb9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95eb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="95eb9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95eb9-108">Permission type</span></span>      | <span data-ttu-id="95eb9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95eb9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95eb9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95eb9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="95eb9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="95eb9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="95eb9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95eb9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95eb9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95eb9-113">Not supported.</span></span>    |
|<span data-ttu-id="95eb9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95eb9-114">Application</span></span> | <span data-ttu-id="95eb9-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="95eb9-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95eb9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95eb9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="95eb9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="95eb9-117">Optional query parameters</span></span>
<span data-ttu-id="95eb9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="95eb9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95eb9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95eb9-119">Request headers</span></span>
| <span data-ttu-id="95eb9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="95eb9-120">Name</span></span>       | <span data-ttu-id="95eb9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="95eb9-121">Type</span></span> | <span data-ttu-id="95eb9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="95eb9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="95eb9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="95eb9-123">Authorization</span></span>  | <span data-ttu-id="95eb9-124">string</span><span class="sxs-lookup"><span data-stu-id="95eb9-124">string</span></span>  | <span data-ttu-id="95eb9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95eb9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95eb9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95eb9-127">Request body</span></span>
<span data-ttu-id="95eb9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95eb9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95eb9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="95eb9-129">Response</span></span>

<span data-ttu-id="95eb9-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95eb9-130">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="95eb9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95eb9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95eb9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95eb9-132">Request</span></span>
<span data-ttu-id="95eb9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95eb9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="95eb9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="95eb9-134">Response</span></span>
<span data-ttu-id="95eb9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95eb9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

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
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="95eb9-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="95eb9-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="95eb9-139">C#</span><span class="sxs-lookup"><span data-stu-id="95eb9-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_serviceprincipal-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95eb9-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="95eb9-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_serviceprincipal-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="95eb9-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95eb9-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_serviceprincipal-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/serviceprincipal-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
