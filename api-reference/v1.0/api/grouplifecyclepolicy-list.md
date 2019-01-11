---
title: Listar groupLifecyclePolicies
description: Listar todos os objetos groupLifecyclePolicies.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 746b6961be84a93201d506639cdf5d586fc5eaf5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804645"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="8ca4c-103">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="8ca4c-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="8ca4c-104">Listar todos os objetos [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ca4c-104">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ca4c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ca4c-105">Permissions</span></span>

<span data-ttu-id="8ca4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ca4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8ca4c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ca4c-108">Permission type</span></span>      | <span data-ttu-id="8ca4c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ca4c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ca4c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ca4c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ca4c-111">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ca4c-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="8ca4c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ca4c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ca4c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ca4c-113">Not supported.</span></span>    |
|<span data-ttu-id="8ca4c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ca4c-114">Application</span></span> | <span data-ttu-id="8ca4c-115">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ca4c-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ca4c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ca4c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8ca4c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8ca4c-117">Optional query parameters</span></span>
<span data-ttu-id="8ca4c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8ca4c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ca4c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ca4c-119">Request headers</span></span>
| <span data-ttu-id="8ca4c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8ca4c-120">Name</span></span> | <span data-ttu-id="8ca4c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ca4c-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="8ca4c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ca4c-122">Authorization</span></span> | <span data-ttu-id="8ca4c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ca4c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ca4c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ca4c-125">Request body</span></span>
<span data-ttu-id="8ca4c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ca4c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ca4c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ca4c-127">Response</span></span>

<span data-ttu-id="8ca4c-128">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ca4c-128">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ca4c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ca4c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8ca4c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ca4c-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="8ca4c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ca4c-131">Response</span></span>

<span data-ttu-id="8ca4c-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ca4c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 223

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 100,
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
