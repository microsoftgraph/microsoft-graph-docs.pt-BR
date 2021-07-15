---
title: 'managementAction: apply'
description: Aplica uma ação de gerenciamento a um locatário gerenciado específico. Ao executar essa operação, as configurações apropriadas serão feitas e as políticas serão criadas. Por exemplo, ao aplicar a autenticação multifacional necessária para a ação de gerenciamento de administradores, criará uma política de acesso condicional Azure Active Directory que requer autenticação multifacional para todos os usuários que foram atribuídos a uma função de diretório administrativo.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 801a4e66338dfb53f74d454c4ac6d2eba2c58505
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442112"
---
# <a name="managementaction-apply"></a><span data-ttu-id="8a6ef-105">managementAction: apply</span><span class="sxs-lookup"><span data-stu-id="8a6ef-105">managementAction: apply</span></span>
<span data-ttu-id="8a6ef-106">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="8a6ef-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a6ef-107">Aplica uma ação de gerenciamento a um locatário gerenciado específico.</span><span class="sxs-lookup"><span data-stu-id="8a6ef-107">Applies a management action against a specific managed tenant.</span></span> <span data-ttu-id="8a6ef-108">Ao executar essa operação, as configurações apropriadas serão feitas e as políticas serão criadas.</span><span class="sxs-lookup"><span data-stu-id="8a6ef-108">By performing this operation the appropriate configurations will be made and policies created.</span></span> <span data-ttu-id="8a6ef-109">Por exemplo, ao aplicar a autenticação multifacional necessária para a ação de gerenciamento de administradores, criará uma política de acesso condicional Azure Active Directory que requer autenticação multifacional para todos os usuários que foram atribuídos a uma função de diretório administrativo.</span><span class="sxs-lookup"><span data-stu-id="8a6ef-109">As example when applying the require multi-factor authentication for admins management action will create an Azure Active Directory conditional access policy that requires multi-factor authentication for all users that have been assigned an administrative directory role.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a6ef-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="8a6ef-110">Permissions</span></span>
<span data-ttu-id="8a6ef-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a6ef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a6ef-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a6ef-113">Permission type</span></span>|<span data-ttu-id="8a6ef-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a6ef-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a6ef-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a6ef-115">Delegated (work or school account)</span></span>|<span data-ttu-id="8a6ef-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a6ef-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="8a6ef-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a6ef-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a6ef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a6ef-118">Not supported.</span></span>|
|<span data-ttu-id="8a6ef-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a6ef-119">Application</span></span>|<span data-ttu-id="8a6ef-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a6ef-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a6ef-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a6ef-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
```

## <a name="request-headers"></a><span data-ttu-id="8a6ef-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a6ef-122">Request headers</span></span>
|<span data-ttu-id="8a6ef-123">Nome</span><span class="sxs-lookup"><span data-stu-id="8a6ef-123">Name</span></span>|<span data-ttu-id="8a6ef-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a6ef-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8a6ef-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a6ef-125">Authorization</span></span>|<span data-ttu-id="8a6ef-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a6ef-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8a6ef-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a6ef-128">Content-Type</span></span>|<span data-ttu-id="8a6ef-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a6ef-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a6ef-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a6ef-131">Request body</span></span>
<span data-ttu-id="8a6ef-132">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8a6ef-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8a6ef-133">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="8a6ef-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8a6ef-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8a6ef-134">Parameter</span></span>|<span data-ttu-id="8a6ef-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a6ef-135">Type</span></span>|<span data-ttu-id="8a6ef-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a6ef-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a6ef-137">tenantId</span><span class="sxs-lookup"><span data-stu-id="8a6ef-137">tenantId</span></span>|<span data-ttu-id="8a6ef-138">String</span><span class="sxs-lookup"><span data-stu-id="8a6ef-138">String</span></span>|<span data-ttu-id="8a6ef-139">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="8a6ef-139">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="8a6ef-140">tenantGroupId</span><span class="sxs-lookup"><span data-stu-id="8a6ef-140">tenantGroupId</span></span>|<span data-ttu-id="8a6ef-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a6ef-141">String</span></span>|<span data-ttu-id="8a6ef-142">O identificador do grupo de locatários.</span><span class="sxs-lookup"><span data-stu-id="8a6ef-142">The identifier of the tenant group.</span></span>|
|<span data-ttu-id="8a6ef-143">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="8a6ef-143">managementTemplateId</span></span>|<span data-ttu-id="8a6ef-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a6ef-144">String</span></span>|<span data-ttu-id="8a6ef-145">O identificador do modelo [de gerenciamento](../resources/managedtenants-managementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="8a6ef-145">The identifier of the [management template](../resources/managedtenants-managementtemplate.md).</span></span>|

## <a name="response"></a><span data-ttu-id="8a6ef-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a6ef-146">Response</span></span>

<span data-ttu-id="8a6ef-147">Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a6ef-147">If successful, this action returns a `200 OK` response code and a [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8a6ef-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8a6ef-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8a6ef-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a6ef-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8a6ef-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a6ef-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "managementaction_apply"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
Content-Type: application/json
Content-length: 95

{
  "tenantId": "String",
  "tenantGroupId": "String",
  "managementTemplateId": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="8a6ef-151">C#</span><span class="sxs-lookup"><span data-stu-id="8a6ef-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/managementaction-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a6ef-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a6ef-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/managementaction-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a6ef-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a6ef-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/managementaction-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a6ef-154">Java</span><span class="sxs-lookup"><span data-stu-id="8a6ef-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/managementaction-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8a6ef-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a6ef-155">Response</span></span>
><span data-ttu-id="8a6ef-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8a6ef-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.managedTenants.ManagementActionDeploymentStatus",
  "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
  "managementActionId": "b22a4713-8428-4952-8cac-d48962ecbdc9",
  "status": "completed",
  "workloadActionDeploymentStatuses": [
    {
      "actionId": "46b80b42-06c7-45b4-b6fb-aa0aecace87b",
      "status": "completed",
      "deployedPolicyId": null,
      "lastDeploymentDateTime": "2021-07-11T19:35:10.4463799Z",
      "error": null
    }
  ]
}
```
