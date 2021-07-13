---
title: Atualizar tenantCustomizedInformation
description: Atualize as propriedades de um objeto tenantCustomizedInformation.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: c9d3c5a812364c5dd8999f89edd4c7ed411db0ab
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401960"
---
# <a name="update-tenantcustomizedinformation"></a><span data-ttu-id="5ae12-103">Atualizar tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="5ae12-103">Update tenantCustomizedInformation</span></span>
<span data-ttu-id="5ae12-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="5ae12-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ae12-105">Atualize as propriedades de [um objeto tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="5ae12-105">Update the properties of a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ae12-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ae12-106">Permissions</span></span>
<span data-ttu-id="5ae12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ae12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ae12-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ae12-109">Permission type</span></span>|<span data-ttu-id="5ae12-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ae12-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ae12-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ae12-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5ae12-112">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae12-112">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="5ae12-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ae12-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ae12-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ae12-114">Not supported.</span></span>|
|<span data-ttu-id="5ae12-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ae12-115">Application</span></span>|<span data-ttu-id="5ae12-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ae12-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ae12-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ae12-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
```

## <a name="request-headers"></a><span data-ttu-id="5ae12-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ae12-118">Request headers</span></span>
|<span data-ttu-id="5ae12-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5ae12-119">Name</span></span>|<span data-ttu-id="5ae12-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ae12-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5ae12-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ae12-121">Authorization</span></span>|<span data-ttu-id="5ae12-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ae12-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5ae12-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ae12-124">Content-Type</span></span>|<span data-ttu-id="5ae12-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ae12-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ae12-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ae12-127">Request body</span></span>
<span data-ttu-id="5ae12-128">No corpo da solicitação, fornece uma representação JSON do [objeto tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="5ae12-128">In the request body, supply a JSON representation of the [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>

<span data-ttu-id="5ae12-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md).</span><span class="sxs-lookup"><span data-stu-id="5ae12-129">The following table shows the properties that are required when you update the [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md).</span></span>

|<span data-ttu-id="5ae12-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ae12-130">Property</span></span>|<span data-ttu-id="5ae12-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ae12-131">Type</span></span>|<span data-ttu-id="5ae12-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ae12-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ae12-133">id</span><span class="sxs-lookup"><span data-stu-id="5ae12-133">id</span></span>|<span data-ttu-id="5ae12-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ae12-134">String</span></span>|<span data-ttu-id="5ae12-135">O Azure Active Directory de locatário do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="5ae12-135">The Azure Active Directory tenant identifier for the managed tenant.</span></span>|
|<span data-ttu-id="5ae12-136">tenantId</span><span class="sxs-lookup"><span data-stu-id="5ae12-136">tenantId</span></span>|<span data-ttu-id="5ae12-137">String</span><span class="sxs-lookup"><span data-stu-id="5ae12-137">String</span></span>|<span data-ttu-id="5ae12-138">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="5ae12-138">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="5ae12-139">contacts</span><span class="sxs-lookup"><span data-stu-id="5ae12-139">contacts</span></span>|<span data-ttu-id="5ae12-140">[coleção microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md)</span><span class="sxs-lookup"><span data-stu-id="5ae12-140">[microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md) collection</span></span>|<span data-ttu-id="5ae12-141">A coleção de contatos associados ao locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="5ae12-141">The collection of contacts associated with the managed tenant.</span></span>|
|<span data-ttu-id="5ae12-142">site</span><span class="sxs-lookup"><span data-stu-id="5ae12-142">website</span></span>|<span data-ttu-id="5ae12-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ae12-143">String</span></span>|<span data-ttu-id="5ae12-144">O site do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="5ae12-144">The website for the managed tenant.</span></span>|

## <a name="response"></a><span data-ttu-id="5ae12-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ae12-145">Response</span></span>

<span data-ttu-id="5ae12-146">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ae12-146">If successful, this method returns a `200 OK` response code and an updated [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ae12-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5ae12-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ae12-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ae12-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tenantcustomizedinformation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
Content-Type: application/json
Content-length: 278

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "tenantId": "String",
  "contacts": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
    }
  ],
  "website": "String"
}
```


### <a name="response"></a><span data-ttu-id="5ae12-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ae12-149">Response</span></span>
><span data-ttu-id="5ae12-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5ae12-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantCustomizedInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
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
}
```
