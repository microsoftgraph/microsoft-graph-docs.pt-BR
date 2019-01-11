---
title: Obter groupLifecyclePolicy
description: Recupera as propriedades e os relacionamentos de um objeto groupLifecyclePolicies.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 0908fea443fbe52185fc3bc2a759cd62cebfa511
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874680"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="13546-103">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="13546-103">Get groupLifecyclePolicy</span></span>

<span data-ttu-id="13546-104">Recupera as propriedades e os relacionamentos de um objeto [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="13546-104">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="13546-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="13546-105">Permissions</span></span>

<span data-ttu-id="13546-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13546-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13546-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13546-108">Permission type</span></span>      | <span data-ttu-id="13546-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13546-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13546-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13546-110">Delegated (work or school account)</span></span> | <span data-ttu-id="13546-111">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13546-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="13546-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13546-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13546-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13546-113">Not supported.</span></span>    |
|<span data-ttu-id="13546-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13546-114">Application</span></span> | <span data-ttu-id="13546-115">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13546-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13546-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13546-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="13546-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="13546-117">Optional query parameters</span></span>
<span data-ttu-id="13546-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="13546-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13546-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13546-119">Request headers</span></span>
| <span data-ttu-id="13546-120">Nome</span><span class="sxs-lookup"><span data-stu-id="13546-120">Name</span></span> | <span data-ttu-id="13546-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="13546-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="13546-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="13546-122">Authorization</span></span> | <span data-ttu-id="13546-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13546-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13546-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13546-125">Request body</span></span>
<span data-ttu-id="13546-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13546-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="13546-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="13546-127">Response</span></span>
<span data-ttu-id="13546-128">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13546-128">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13546-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13546-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="13546-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13546-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="13546-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="13546-131">Response</span></span>

<span data-ttu-id="13546-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13546-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
