---
title: Atualizar tenantCustomizedInformation
description: Atualize as propriedades de um objeto tenantCustomizedInformation.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 3f43e7e3f543c0a74b27a3594f573d4fe3cc68c6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441791"
---
# <a name="update-tenantcustomizedinformation"></a><span data-ttu-id="f62da-103">Atualizar tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="f62da-103">Update tenantCustomizedInformation</span></span>
<span data-ttu-id="f62da-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f62da-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f62da-105">Atualize as propriedades de [um objeto tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="f62da-105">Update the properties of a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f62da-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f62da-106">Permissions</span></span>
<span data-ttu-id="f62da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f62da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f62da-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f62da-109">Permission type</span></span>|<span data-ttu-id="f62da-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f62da-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f62da-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f62da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f62da-112">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f62da-112">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="f62da-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f62da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f62da-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f62da-114">Not supported.</span></span>|
|<span data-ttu-id="f62da-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f62da-115">Application</span></span>|<span data-ttu-id="f62da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f62da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f62da-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f62da-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
```

## <a name="request-headers"></a><span data-ttu-id="f62da-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f62da-118">Request headers</span></span>
|<span data-ttu-id="f62da-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f62da-119">Name</span></span>|<span data-ttu-id="f62da-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f62da-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f62da-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f62da-121">Authorization</span></span>|<span data-ttu-id="f62da-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f62da-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f62da-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f62da-124">Content-Type</span></span>|<span data-ttu-id="f62da-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f62da-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f62da-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f62da-127">Request body</span></span>
<span data-ttu-id="f62da-128">No corpo da solicitação, fornece uma representação JSON do [objeto tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="f62da-128">In the request body, supply a JSON representation of the [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>

<span data-ttu-id="f62da-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md).</span><span class="sxs-lookup"><span data-stu-id="f62da-129">The following table shows the properties that are required when you update the [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md).</span></span>

|<span data-ttu-id="f62da-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f62da-130">Property</span></span>|<span data-ttu-id="f62da-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f62da-131">Type</span></span>|<span data-ttu-id="f62da-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f62da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f62da-133">id</span><span class="sxs-lookup"><span data-stu-id="f62da-133">id</span></span>|<span data-ttu-id="f62da-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f62da-134">String</span></span>|<span data-ttu-id="f62da-135">O Azure Active Directory de locatário do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f62da-135">The Azure Active Directory tenant identifier for the managed tenant.</span></span>|
|<span data-ttu-id="f62da-136">tenantId</span><span class="sxs-lookup"><span data-stu-id="f62da-136">tenantId</span></span>|<span data-ttu-id="f62da-137">String</span><span class="sxs-lookup"><span data-stu-id="f62da-137">String</span></span>|<span data-ttu-id="f62da-138">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="f62da-138">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="f62da-139">contacts</span><span class="sxs-lookup"><span data-stu-id="f62da-139">contacts</span></span>|<span data-ttu-id="f62da-140">[coleção microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md)</span><span class="sxs-lookup"><span data-stu-id="f62da-140">[microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md) collection</span></span>|<span data-ttu-id="f62da-141">A coleção de contatos associados ao locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f62da-141">The collection of contacts associated with the managed tenant.</span></span>|
|<span data-ttu-id="f62da-142">site</span><span class="sxs-lookup"><span data-stu-id="f62da-142">website</span></span>|<span data-ttu-id="f62da-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f62da-143">String</span></span>|<span data-ttu-id="f62da-144">O site do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f62da-144">The website for the managed tenant.</span></span>|

## <a name="response"></a><span data-ttu-id="f62da-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f62da-145">Response</span></span>

<span data-ttu-id="f62da-146">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f62da-146">If successful, this method returns a `200 OK` response code and an updated [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f62da-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f62da-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f62da-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f62da-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f62da-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="f62da-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f62da-150">C#</span><span class="sxs-lookup"><span data-stu-id="f62da-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenantcustomizedinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f62da-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f62da-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenantcustomizedinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f62da-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f62da-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenantcustomizedinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f62da-153">Java</span><span class="sxs-lookup"><span data-stu-id="f62da-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenantcustomizedinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f62da-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f62da-154">Response</span></span>
><span data-ttu-id="f62da-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f62da-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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
