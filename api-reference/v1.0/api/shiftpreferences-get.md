---
title: Obter shiftPreferences
description: Obter uma preferência de turno por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a4ee1518048931d605acfb4dd96908285fc44b9b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034851"
---
# <a name="get-shiftpreferences"></a><span data-ttu-id="e41db-103">Obter shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="e41db-103">Get shiftPreferences</span></span>

<span data-ttu-id="e41db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e41db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e41db-105">Recupere as propriedades e as relações de um [objeto shiftPreferences](../resources/shiftpreferences.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="e41db-105">Retrieve the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="e41db-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e41db-106">Permissions</span></span>

<span data-ttu-id="e41db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e41db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e41db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e41db-109">Permission type</span></span>      | <span data-ttu-id="e41db-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e41db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e41db-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e41db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e41db-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e41db-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="e41db-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e41db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e41db-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e41db-114">Not supported.</span></span>    |
|<span data-ttu-id="e41db-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e41db-115">Application</span></span> | <span data-ttu-id="e41db-116">UserShiftPreferences.Read.All, UserShiftPreferences.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e41db-116">UserShiftPreferences.Read.All, UserShiftPreferences.ReadWrite.All</span></span> |

> <span data-ttu-id="e41db-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="e41db-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e41db-118">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="e41db-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e41db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e41db-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e41db-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e41db-120">Optional query parameters</span></span>

<span data-ttu-id="e41db-121">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e41db-121">This method does not support OData query parameters to customize the response.</span></span>


## <a name="request-headers"></a><span data-ttu-id="e41db-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e41db-122">Request headers</span></span>

| <span data-ttu-id="e41db-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e41db-123">Header</span></span>       | <span data-ttu-id="e41db-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e41db-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e41db-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e41db-125">Authorization</span></span>  | <span data-ttu-id="e41db-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e41db-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e41db-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e41db-128">Request body</span></span>
<span data-ttu-id="e41db-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e41db-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e41db-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e41db-130">Response</span></span>

<span data-ttu-id="e41db-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto shiftPreferences](../resources/shiftpreferences.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e41db-131">If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e41db-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e41db-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e41db-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e41db-133">Request</span></span>

<span data-ttu-id="e41db-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e41db-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e41db-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e41db-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_shiftpreferences"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences
```
# <a name="c"></a>[<span data-ttu-id="e41db-136">C#</span><span class="sxs-lookup"><span data-stu-id="e41db-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shiftpreferences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e41db-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e41db-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shiftpreferences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e41db-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e41db-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shiftpreferences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e41db-139">Java</span><span class="sxs-lookup"><span data-stu-id="e41db-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shiftpreferences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e41db-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e41db-140">Response</span></span>

<span data-ttu-id="e41db-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e41db-141">The following is an example of the response.</span></span>

><span data-ttu-id="e41db-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e41db-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shiftPreferences"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "id": "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7",
    "@odata.etag": "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa",
    "availability": [
        {
            "recurrence": {
                "pattern": {
                    "type": "Weekly",
                    "daysOfWeek": ["Tuesday"],
                    "interval": 1
                },
                "range": {
                    "type": "noEnd"
                }
            },
            "timeZone": "Pacific Standard Time",
            "timeSlots": [
                {
                    "startTime": "09:15:00.000000",
                    "endTime": "12:30:00.000000"
                },
                {
                    "startTime": "16:00:00.000000",
                    "endTime": "20:00:00.000000"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-12-12 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a user's shift preferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

