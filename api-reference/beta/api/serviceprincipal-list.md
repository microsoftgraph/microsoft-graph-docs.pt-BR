---
title: List servicePrincipals
description: Recupere uma lista de objetos servicePrincipal.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 728766ae1bb092ce1e5783f2d6adc08860928c67
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218637"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="05e70-103">List servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="05e70-103">List servicePrincipals</span></span>

<span data-ttu-id="05e70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05e70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05e70-105">Recupere uma lista de objetos servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="05e70-105">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="05e70-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="05e70-106">Permissions</span></span>

<span data-ttu-id="05e70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05e70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="05e70-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05e70-109">Permission type</span></span>      | <span data-ttu-id="05e70-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05e70-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05e70-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05e70-111">Delegated (work or school account)</span></span> | <span data-ttu-id="05e70-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="05e70-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05e70-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05e70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05e70-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05e70-114">Not supported.</span></span>    |
|<span data-ttu-id="05e70-115">Application</span><span class="sxs-lookup"><span data-stu-id="05e70-115">Application</span></span> | <span data-ttu-id="05e70-116">Application. Read. All, Application. ReadWrite. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="05e70-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05e70-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05e70-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="05e70-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="05e70-118">Optional query parameters</span></span>

<span data-ttu-id="05e70-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="05e70-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05e70-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05e70-120">Request headers</span></span>
| <span data-ttu-id="05e70-121">Nome</span><span class="sxs-lookup"><span data-stu-id="05e70-121">Name</span></span> | <span data-ttu-id="05e70-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="05e70-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="05e70-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="05e70-123">Authorization</span></span>  | <span data-ttu-id="05e70-124">string</span><span class="sxs-lookup"><span data-stu-id="05e70-124">string</span></span>  | <span data-ttu-id="05e70-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05e70-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05e70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05e70-127">Request body</span></span>

<span data-ttu-id="05e70-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05e70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05e70-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="05e70-129">Response</span></span>

<span data-ttu-id="05e70-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos de [servicePrincipalName](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05e70-130">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05e70-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05e70-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="05e70-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05e70-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="05e70-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="05e70-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals
```
# <a name="c"></a>[<span data-ttu-id="05e70-134">C#</span><span class="sxs-lookup"><span data-stu-id="05e70-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05e70-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05e70-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05e70-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05e70-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="05e70-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="05e70-137">Response</span></span>

<span data-ttu-id="05e70-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05e70-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
