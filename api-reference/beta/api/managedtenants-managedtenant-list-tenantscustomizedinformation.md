---
title: Listar tenantCustomizedInformation
description: Obter uma lista dos objetos tenantCustomizedInformation e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 5aebbe468adab64b90889587142ec354330ba93c
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402102"
---
# <a name="list-tenantcustomizedinformation"></a><span data-ttu-id="81fb8-103">Listar tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="81fb8-103">List tenantCustomizedInformation</span></span>
<span data-ttu-id="81fb8-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="81fb8-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81fb8-105">Obter uma lista dos [objetos tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="81fb8-105">Get a list of the [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="81fb8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81fb8-106">Permissions</span></span>
<span data-ttu-id="81fb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81fb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81fb8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81fb8-109">Permission type</span></span>|<span data-ttu-id="81fb8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81fb8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81fb8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81fb8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81fb8-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81fb8-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="81fb8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81fb8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81fb8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81fb8-114">Not supported.</span></span>|
|<span data-ttu-id="81fb8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81fb8-115">Application</span></span>|<span data-ttu-id="81fb8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81fb8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81fb8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81fb8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantsCustomizedInformation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81fb8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="81fb8-118">Optional query parameters</span></span>
<span data-ttu-id="81fb8-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="81fb8-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81fb8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81fb8-120">Request headers</span></span>
|<span data-ttu-id="81fb8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="81fb8-121">Name</span></span>|<span data-ttu-id="81fb8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="81fb8-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="81fb8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="81fb8-123">Authorization</span></span>|<span data-ttu-id="81fb8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81fb8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81fb8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81fb8-126">Request body</span></span>
<span data-ttu-id="81fb8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81fb8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81fb8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="81fb8-128">Response</span></span>

<span data-ttu-id="81fb8-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81fb8-129">If successful, this method returns a `200 OK` response code and a collection of [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81fb8-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="81fb8-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81fb8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81fb8-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_tenantcustomizedinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsCustomizedInformation
```


### <a name="response"></a><span data-ttu-id="81fb8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="81fb8-132">Response</span></span>
><span data-ttu-id="81fb8-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="81fb8-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantCustomizedInformation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/managedTenants/$metadata#tenantCustomizedInformation",
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "website": "https://www.fourthcoffee.com",
      "contacts": [
        {
          "name": "Sally",
          "email": "sally@fourthcoffee.com",
          "phone": "5558009731"
        },
        {
          "name": "Hector",
          "email": "hector@fourthcoffee.com",
          "phone": "5558009732"
        }
      ]
    },
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320\",",
      "website": "https://www.consolidatedmessenger.com",
      "contacts": [
        {
          "name": "Cynthia",
          "email": "cynthia@consolidatedmessenger.com",
          "phone": "5558001370"
        },
        {
          "name": "Timothy",
          "email": "timothy@consolidatedmessenger.com",
          "phone": "5558001379"
        }
      ]
    }
  ]
}
```
