---
title: Criar tenantTag
description: Crie um novo objeto tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 9de058914e2262debcbe87d449b5ffc7fc15db7b
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402017"
---
# <a name="create-tenanttag"></a><span data-ttu-id="5d906-103">Criar tenantTag</span><span class="sxs-lookup"><span data-stu-id="5d906-103">Create tenantTag</span></span>
<span data-ttu-id="5d906-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="5d906-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d906-105">Crie um novo [objeto tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="5d906-105">Create a new [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d906-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d906-106">Permissions</span></span>
<span data-ttu-id="5d906-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d906-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d906-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d906-109">Permission type</span></span>|<span data-ttu-id="5d906-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d906-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d906-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d906-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5d906-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="5d906-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="5d906-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d906-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d906-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d906-114">Not supported.</span></span>|
|<span data-ttu-id="5d906-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d906-115">Application</span></span>|<span data-ttu-id="5d906-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d906-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d906-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d906-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags
```

## <a name="request-headers"></a><span data-ttu-id="5d906-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d906-118">Request headers</span></span>
|<span data-ttu-id="5d906-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5d906-119">Name</span></span>|<span data-ttu-id="5d906-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d906-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5d906-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d906-121">Authorization</span></span>|<span data-ttu-id="5d906-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d906-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5d906-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d906-124">Content-Type</span></span>|<span data-ttu-id="5d906-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d906-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d906-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d906-127">Request body</span></span>
<span data-ttu-id="5d906-128">No corpo da solicitação, fornece uma representação JSON do [objeto tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="5d906-128">In the request body, supply a JSON representation of the [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

<span data-ttu-id="5d906-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [a tenantTag](../resources/managedtenants-tenanttag.md).</span><span class="sxs-lookup"><span data-stu-id="5d906-129">The following table shows the properties that are required when you create the [tenantTag](../resources/managedtenants-tenanttag.md).</span></span>

|<span data-ttu-id="5d906-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d906-130">Property</span></span>|<span data-ttu-id="5d906-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d906-131">Type</span></span>|<span data-ttu-id="5d906-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d906-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d906-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5d906-133">displayName</span></span>|<span data-ttu-id="5d906-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d906-134">String</span></span>|<span data-ttu-id="5d906-135">O nome de exibição da marca de locatário.</span><span class="sxs-lookup"><span data-stu-id="5d906-135">The display name for the tenant tag.</span></span>|
|<span data-ttu-id="5d906-136">description</span><span class="sxs-lookup"><span data-stu-id="5d906-136">description</span></span>|<span data-ttu-id="5d906-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d906-137">String</span></span>|<span data-ttu-id="5d906-138">A descrição da marca de locatário.</span><span class="sxs-lookup"><span data-stu-id="5d906-138">The description for the tenant tag.</span></span>|

## <a name="response"></a><span data-ttu-id="5d906-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d906-139">Response</span></span>

<span data-ttu-id="5d906-140">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [tenantTag](../resources/managedtenants-tenanttag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d906-140">If successful, this method returns a `201 Created` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d906-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5d906-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d906-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d906-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tenanttag_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags
Content-Type: application/json
Content-length: 382

{
  "displayName": "Support",
  "description": "Tenants that have purchased extended support"
}
```

### <a name="response"></a><span data-ttu-id="5d906-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d906-143">Response</span></span>
><span data-ttu-id="5d906-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5d906-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "11103b2b-0e28-456b-901d-45f98890ab1d",
  "displayName": "Support",
  "description": "Tenants that have purchased extended support",
  "tenantIds": [],
  "isDeleted": null,
  "createdDateTime": "2021-07-11T19:31:49.807267Z",
  "createdByUserId": "cad28f13-0158-43c5-9c59-952f2caa62c0",
  "lastActionDateTime": "2021-07-11T19:31:49.8072716Z",
  "lastActionByUserId": "cad28f13-0158-43c5-9c59-952f2caa62c0"
}
```
