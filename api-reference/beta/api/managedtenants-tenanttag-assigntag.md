---
title: 'tenantTag: assignTag'
description: Atribua a marca de locatário aos locatários gerenciados especificados.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 8f9d641cb0d3129802431948601d656f9036e2ef
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402108"
---
# <a name="tenanttag-assigntag"></a><span data-ttu-id="a5d1c-103">tenantTag: assignTag</span><span class="sxs-lookup"><span data-stu-id="a5d1c-103">tenantTag: assignTag</span></span>
<span data-ttu-id="a5d1c-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="a5d1c-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5d1c-105">Atribua a marca de locatário aos locatários gerenciados especificados.</span><span class="sxs-lookup"><span data-stu-id="a5d1c-105">Assign the tenant tag to the specified managed tenants.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5d1c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5d1c-106">Permissions</span></span>
<span data-ttu-id="a5d1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5d1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5d1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5d1c-109">Permission type</span></span>|<span data-ttu-id="a5d1c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5d1c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5d1c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5d1c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a5d1c-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="a5d1c-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="a5d1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5d1c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5d1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5d1c-114">Not supported.</span></span>|
|<span data-ttu-id="a5d1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5d1c-115">Application</span></span>|<span data-ttu-id="a5d1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5d1c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5d1c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5d1c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags/{tenantTagId}/assignTag
```

## <a name="request-headers"></a><span data-ttu-id="a5d1c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5d1c-118">Request headers</span></span>
|<span data-ttu-id="a5d1c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a5d1c-119">Name</span></span>|<span data-ttu-id="a5d1c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5d1c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a5d1c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5d1c-121">Authorization</span></span>|<span data-ttu-id="a5d1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5d1c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a5d1c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5d1c-124">Content-Type</span></span>|<span data-ttu-id="a5d1c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5d1c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5d1c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5d1c-127">Request body</span></span>
<span data-ttu-id="a5d1c-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a5d1c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a5d1c-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="a5d1c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a5d1c-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a5d1c-130">Parameter</span></span>|<span data-ttu-id="a5d1c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5d1c-131">Type</span></span>|<span data-ttu-id="a5d1c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5d1c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5d1c-133">tenantIds</span><span class="sxs-lookup"><span data-stu-id="a5d1c-133">tenantIds</span></span>|<span data-ttu-id="a5d1c-134">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5d1c-134">String collection</span></span>|<span data-ttu-id="a5d1c-135">A coleção de Azure Active Directory de locatários onde a marca de locatário deve ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="a5d1c-135">The collection of Azure Active Directory tenant identifiers where the tenant tag should be assigned.</span></span>|

## <a name="response"></a><span data-ttu-id="a5d1c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5d1c-136">Response</span></span>

<span data-ttu-id="a5d1c-137">Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [tenantTag](../resources/managedtenants-tenanttag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5d1c-137">If successful, this action returns a `200 OK` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5d1c-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a5d1c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5d1c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5d1c-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "tenanttag_assigntag"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}/assignTag
Content-Type: application/json
Content-length: 41

{
  "tenantIds": [
    "String"
  ]
}
```

### <a name="response"></a><span data-ttu-id="a5d1c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5d1c-140">Response</span></span>
><span data-ttu-id="a5d1c-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a5d1c-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "displayName": "Support",
  "description": "Tenants that have purchased support",
  "tenants": [
    {
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
    }
  ],
  "isDeleted": null,
  "createdDateTime": "2021-06-26T13:51:23.3927236Z",
  "createdByUserId": "65ca7649-4ccb-4823-9c39-42bd75191bf8",
  "lastActionDateTime": "2021-07-11T19:55:19.7230386Z",
  "lastActionByUserId": "50bf7bd8-1b3a-4d1d-94c5-86d27e68857f"
}
```
