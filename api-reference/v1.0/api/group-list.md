---
title: Listar grupos
description: Lista todos os grupos disponíveis em uma organização, incluindo, mas não limitando-se a, grupos do Office 365.
localization_priority: Priority
ms.openlocfilehash: 1122685cfbd4f1a1f2ff0ca3367e913c983866a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867715"
---
# <a name="list-groups"></a><span data-ttu-id="1a8f7-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="1a8f7-103">List groups</span></span>
<span data-ttu-id="1a8f7-p101">Lista todos os grupos disponíveis em uma organização, incluindo, mas não limitando-se a, grupos do Office 365. As [propriedades padrão](../api/group-get.md#default-properties) de cada grupo são retornadas.</span><span class="sxs-lookup"><span data-stu-id="1a8f7-p101">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group-get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="1a8f7-106">Para listar apenas grupos do Office 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="1a8f7-106">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="1a8f7-107">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="1a8f7-107">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

## <a name="permissions"></a><span data-ttu-id="1a8f7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a8f7-108">Permissions</span></span>
<span data-ttu-id="1a8f7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a8f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a8f7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a8f7-111">Permission type</span></span>      | <span data-ttu-id="1a8f7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a8f7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a8f7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a8f7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1a8f7-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a8f7-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a8f7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a8f7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a8f7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a8f7-116">Not supported.</span></span>    |
|<span data-ttu-id="1a8f7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a8f7-117">Application</span></span> | <span data-ttu-id="1a8f7-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a8f7-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a8f7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a8f7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a8f7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1a8f7-120">Optional query parameters</span></span>
<span data-ttu-id="1a8f7-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1a8f7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a8f7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a8f7-122">Request headers</span></span>
| <span data-ttu-id="1a8f7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1a8f7-123">Name</span></span>       | <span data-ttu-id="1a8f7-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a8f7-124">Type</span></span> | <span data-ttu-id="1a8f7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a8f7-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1a8f7-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a8f7-126">Authorization</span></span>  | <span data-ttu-id="1a8f7-127">string</span><span class="sxs-lookup"><span data-stu-id="1a8f7-127">string</span></span>  | <span data-ttu-id="1a8f7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a8f7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a8f7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a8f7-130">Request body</span></span>
<span data-ttu-id="1a8f7-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a8f7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a8f7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a8f7-132">Response</span></span>
<span data-ttu-id="1a8f7-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a8f7-133">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a8f7-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a8f7-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1a8f7-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a8f7-135">Request</span></span>
<span data-ttu-id="1a8f7-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a8f7-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="1a8f7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a8f7-137">Response</span></span>
<span data-ttu-id="1a8f7-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a8f7-138">The following is an example of the response.</span></span>

><span data-ttu-id="1a8f7-139">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1a8f7-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1a8f7-140">As [propriedades padrão](../api/group-get.md#default-properties) serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a8f7-140">The [default properties](../api/group-get.md#default-properties) will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
    {
      "id": "id-value",
      "description": "description-value",
      "displayName": "displayName-value",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "mailEnabled": true,
      "mailNickname": "mailNickname-value",
      "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
      "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
      "onPremisesSyncEnabled": true,
      "proxyAddresses": [
        "proxyAddresses-value"
      ],
      "securityEnabled": true,
      "visibility": "visibility-value"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
