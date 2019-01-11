---
title: Listar groupLifecyclePolicies
description: Recupera uma lista de objetos groupLifecyclePolicy à qual um grupo pertence.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 7bcb01b35a7d2c39dd02cd54ff5287f893524521
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875534"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="389ff-103">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="389ff-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="389ff-104">Recupera uma lista de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) à qual um grupo pertence.</span><span class="sxs-lookup"><span data-stu-id="389ff-104">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="389ff-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="389ff-105">Permissions</span></span>

<span data-ttu-id="389ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="389ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="389ff-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="389ff-108">Permission type</span></span>      | <span data-ttu-id="389ff-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="389ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="389ff-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="389ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="389ff-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="389ff-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="389ff-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="389ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="389ff-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="389ff-113">Not supported.</span></span>    |
|<span data-ttu-id="389ff-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="389ff-114">Application</span></span> | <span data-ttu-id="389ff-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="389ff-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="389ff-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="389ff-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="389ff-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="389ff-117">Optional query parameters</span></span>
<span data-ttu-id="389ff-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="389ff-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="389ff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="389ff-119">Request headers</span></span>
| <span data-ttu-id="389ff-120">Nome</span><span class="sxs-lookup"><span data-stu-id="389ff-120">Name</span></span> | <span data-ttu-id="389ff-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="389ff-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="389ff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="389ff-122">Authorization</span></span> | <span data-ttu-id="389ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="389ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="389ff-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="389ff-125">Request body</span></span>
<span data-ttu-id="389ff-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="389ff-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="389ff-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="389ff-127">Response</span></span>
<span data-ttu-id="389ff-128">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="389ff-128">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="389ff-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="389ff-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="389ff-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="389ff-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="389ff-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="389ff-131">Response</span></span>

<span data-ttu-id="389ff-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="389ff-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 90,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
