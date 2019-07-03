---
title: List servicePrincipals
description: Recupere uma lista de objetos servicePrincipal.
localization_priority: Normal
ms.openlocfilehash: 8f1ba69fcea65fb96d95b497121466e4a50ddc66
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453737"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="d3a2b-103">List servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="d3a2b-103">List servicePrincipals</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3a2b-104">Recupere uma lista de objetos servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="d3a2b-104">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3a2b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3a2b-105">Permissions</span></span>

<span data-ttu-id="d3a2b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3a2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d3a2b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3a2b-108">Permission type</span></span>      | <span data-ttu-id="d3a2b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3a2b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3a2b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3a2b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d3a2b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d3a2b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d3a2b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3a2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3a2b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3a2b-113">Not supported.</span></span>    |
|<span data-ttu-id="d3a2b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3a2b-114">Application</span></span> | <span data-ttu-id="d3a2b-115">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3a2b-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3a2b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3a2b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d3a2b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d3a2b-117">Optional query parameters</span></span>

<span data-ttu-id="d3a2b-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d3a2b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3a2b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a2b-119">Request headers</span></span>
| <span data-ttu-id="d3a2b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d3a2b-120">Name</span></span> | <span data-ttu-id="d3a2b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3a2b-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="d3a2b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3a2b-122">Authorization</span></span>  | <span data-ttu-id="d3a2b-123">string</span><span class="sxs-lookup"><span data-stu-id="d3a2b-123">string</span></span>  | <span data-ttu-id="d3a2b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3a2b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3a2b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a2b-126">Request body</span></span>

<span data-ttu-id="d3a2b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3a2b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3a2b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3a2b-128">Response</span></span>

<span data-ttu-id="d3a2b-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos de [servicePrincipalName](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3a2b-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3a2b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3a2b-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d3a2b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a2b-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d3a2b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3a2b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d3a2b-133">C#</span><span class="sxs-lookup"><span data-stu-id="d3a2b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3a2b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3a2b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d3a2b-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d3a2b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d3a2b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3a2b-136">Response</span></span>

<span data-ttu-id="d3a2b-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3a2b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
