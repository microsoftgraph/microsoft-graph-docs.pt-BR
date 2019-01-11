---
title: Listar grupos
description: Lista todos os grupos disponíveis em uma organização, incluindo, mas não limitando-se a, grupos do Office 365.
localization_priority: Priority
ms.openlocfilehash: dd243d1f07b98564bb5aa4751664337c0f0654cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813269"
---
# <a name="list-groups"></a><span data-ttu-id="3aa65-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="3aa65-103">List groups</span></span>

> <span data-ttu-id="3aa65-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3aa65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3aa65-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3aa65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3aa65-p102">Lista todos os grupos disponíveis em uma organização, incluindo, mas não limitando-se a, grupos do Office 365. As [propriedades padrão](../api/group-get.md#default-properties) de cada grupo são retornadas.</span><span class="sxs-lookup"><span data-stu-id="3aa65-p102">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group-get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="3aa65-108">Para listar apenas grupos do Office 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="3aa65-108">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="3aa65-109">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="3aa65-109">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="3aa65-110">Para retornar os grupos que contêm membros com erros de licença, use o parâmetro de consulta **$filter** :</span><span class="sxs-lookup"><span data-stu-id="3aa65-110">To return groups containing members with license errors, use the **$filter** query parameter:</span></span> 

```http 
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true 
```
## <a name="permissions"></a><span data-ttu-id="3aa65-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="3aa65-111">Permissions</span></span>
<span data-ttu-id="3aa65-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aa65-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aa65-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3aa65-114">Permission type</span></span>      | <span data-ttu-id="3aa65-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3aa65-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3aa65-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3aa65-116">Delegated (work or school account)</span></span> | <span data-ttu-id="3aa65-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aa65-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3aa65-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3aa65-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aa65-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3aa65-119">Not supported.</span></span>    |
|<span data-ttu-id="3aa65-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3aa65-120">Application</span></span> | <span data-ttu-id="3aa65-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aa65-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3aa65-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3aa65-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3aa65-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3aa65-123">Optional query parameters</span></span>
<span data-ttu-id="3aa65-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3aa65-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3aa65-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3aa65-125">Request headers</span></span>
| <span data-ttu-id="3aa65-126">Nome</span><span class="sxs-lookup"><span data-stu-id="3aa65-126">Name</span></span>       | <span data-ttu-id="3aa65-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="3aa65-127">Type</span></span> | <span data-ttu-id="3aa65-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aa65-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3aa65-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="3aa65-129">Authorization</span></span>  | <span data-ttu-id="3aa65-130">string</span><span class="sxs-lookup"><span data-stu-id="3aa65-130">string</span></span>  | <span data-ttu-id="3aa65-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3aa65-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3aa65-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3aa65-133">Request body</span></span>
<span data-ttu-id="3aa65-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3aa65-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3aa65-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aa65-135">Response</span></span>
<span data-ttu-id="3aa65-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3aa65-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aa65-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3aa65-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3aa65-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aa65-138">Request</span></span>
<span data-ttu-id="3aa65-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aa65-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```

#### <a name="response"></a><span data-ttu-id="3aa65-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aa65-140">Response</span></span>
<span data-ttu-id="3aa65-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3aa65-141">The following is an example of the response.</span></span>
><span data-ttu-id="3aa65-142">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3aa65-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3aa65-143">As [propriedades padrão](../api/group-get.md#default-properties) serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3aa65-143">The [default properties](../api/group-get.md#default-properties) will be returned from an actual call.</span></span>

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
