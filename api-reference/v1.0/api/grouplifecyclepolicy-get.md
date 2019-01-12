---
title: Obter groupLifecyclePolicy
description: Recupera as propriedades e os relacionamentos de um objeto groupLifecyclePolicies.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0b4d29ca8a08c2ec805549e6f10da4ac268771a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917927"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="5a09f-103">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="5a09f-103">Get groupLifecyclePolicy</span></span>

<span data-ttu-id="5a09f-104">Recupera as propriedades e os relacionamentos de um objeto [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5a09f-104">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a09f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a09f-105">Permissions</span></span>

<span data-ttu-id="5a09f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a09f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a09f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a09f-108">Permission type</span></span>      | <span data-ttu-id="5a09f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a09f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a09f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a09f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a09f-111">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a09f-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="5a09f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a09f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a09f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a09f-113">Not supported.</span></span>    |
|<span data-ttu-id="5a09f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a09f-114">Application</span></span> | <span data-ttu-id="5a09f-115">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a09f-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a09f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a09f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5a09f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5a09f-117">Optional query parameters</span></span>
<span data-ttu-id="5a09f-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5a09f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a09f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a09f-119">Request headers</span></span>
| <span data-ttu-id="5a09f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5a09f-120">Name</span></span> | <span data-ttu-id="5a09f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a09f-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="5a09f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a09f-122">Authorization</span></span> | <span data-ttu-id="5a09f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a09f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a09f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a09f-125">Request body</span></span>
<span data-ttu-id="5a09f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a09f-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5a09f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a09f-127">Response</span></span>
<span data-ttu-id="5a09f-128">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a09f-128">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5a09f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a09f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5a09f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a09f-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="5a09f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a09f-131">Response</span></span>

<span data-ttu-id="5a09f-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a09f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
