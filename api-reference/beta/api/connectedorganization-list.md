---
title: Listar connectedOrganizations
description: Recupere uma lista de objetos connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b685b6e9b81a8a861f3c1a2da4aabccb43272c83
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509940"
---
# <a name="list-connectedorganizations"></a><span data-ttu-id="f5ffa-103">Listar connectedOrganizations</span><span class="sxs-lookup"><span data-stu-id="f5ffa-103">List connectedOrganizations</span></span>

<span data-ttu-id="f5ffa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5ffa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5ffa-105">Recupere uma lista de objetos [connectedOrganization](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="f5ffa-105">Retrieve a list of [connectedOrganization](../resources/connectedorganization.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5ffa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5ffa-106">Permissions</span></span>

<span data-ttu-id="f5ffa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5ffa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5ffa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5ffa-109">Permission type</span></span>|<span data-ttu-id="f5ffa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5ffa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="f5ffa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5ffa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5ffa-112">EntitlementManagement. Read. All, EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f5ffa-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f5ffa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5ffa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5ffa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5ffa-114">Not supported.</span></span> |
| <span data-ttu-id="f5ffa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5ffa-115">Application</span></span>                            | <span data-ttu-id="f5ffa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5ffa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5ffa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5ffa-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f5ffa-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f5ffa-118">Optional query parameters</span></span>
<span data-ttu-id="f5ffa-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f5ffa-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f5ffa-120">Por exemplo, para recuperar apenas as organizações conectadas com um nome de exibição específico, adicione `$filter=displayName eq 'Name'` .</span><span class="sxs-lookup"><span data-stu-id="f5ffa-120">For example, to retrieve only the connected organizations with a specific display name, add `$filter=displayName eq 'Name'`.</span></span> <span data-ttu-id="f5ffa-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f5ffa-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5ffa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ffa-122">Request headers</span></span>
|<span data-ttu-id="f5ffa-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f5ffa-123">Name</span></span>|<span data-ttu-id="f5ffa-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5ffa-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f5ffa-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5ffa-125">Authorization</span></span>|<span data-ttu-id="f5ffa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5ffa-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5ffa-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ffa-128">Request body</span></span>
<span data-ttu-id="f5ffa-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5ffa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5ffa-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ffa-130">Response</span></span>

<span data-ttu-id="f5ffa-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [connectedOrganization](../resources/connectedorganization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5ffa-131">If successful, this method returns a `200 OK` response code and a collection of [connectedOrganization](../resources/connectedorganization.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5ffa-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f5ffa-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5ffa-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ffa-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectedorganizations"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations
```

### <a name="response"></a><span data-ttu-id="f5ffa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ffa-134">Response</span></span>
<span data-ttu-id="f5ffa-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f5ffa-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.connectedOrganization)"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "cd3709c6-be6a-4725-bd07-50f90ccca93f",
      "displayName": "Wingtip Toys",
      "description": "Wingtip Toys",
      "createdBy": "admin@contoso.com",
      "createdDateTime": "2020-05-13T15:18:04.81Z",
      "modifiedBy": "admin@contoso.com",
      "modifiedDateTime": "2020-05-13T15:18:04.81Z",
      "identitySources": [
        {
          "@odata.type": "#microsoft.graph.azureActiveDirectoryTenant",
          "tenantId": "bf85dc9d-cb43-44a4-80c4-469e8c58249e",
          "displayName": "Wingtip Toys Co"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connectedOrganizations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
