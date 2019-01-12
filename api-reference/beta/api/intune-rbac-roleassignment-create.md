---
title: Criar roleAssignment
description: Criar um novo objeto roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1c6dc9bf1bbc819b2e74a7e55defadda177bf67d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920363"
---
# <a name="create-roleassignment"></a><span data-ttu-id="7cc0c-103">Criar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="7cc0c-103">Create roleAssignment</span></span>

> <span data-ttu-id="7cc0c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cc0c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7cc0c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cc0c-107">Criar um novo objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7cc0c-107">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cc0c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7cc0c-108">Prerequisites</span></span>
<span data-ttu-id="7cc0c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cc0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cc0c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cc0c-111">Permission type</span></span>|<span data-ttu-id="7cc0c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7cc0c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cc0c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cc0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7cc0c-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cc0c-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="7cc0c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cc0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cc0c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-116">Not supported.</span></span>|
|<span data-ttu-id="7cc0c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cc0c-117">Application</span></span>|<span data-ttu-id="7cc0c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cc0c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cc0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="7cc0c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cc0c-120">Request headers</span></span>
|<span data-ttu-id="7cc0c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7cc0c-121">Header</span></span>|<span data-ttu-id="7cc0c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7cc0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cc0c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cc0c-123">Authorization</span></span>|<span data-ttu-id="7cc0c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cc0c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7cc0c-125">Accept</span></span>|<span data-ttu-id="7cc0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7cc0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cc0c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cc0c-127">Request body</span></span>
<span data-ttu-id="7cc0c-128">No corpo da solicitação, forneça uma representação JSON do objeto roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-128">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="7cc0c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-129">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="7cc0c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7cc0c-130">Property</span></span>|<span data-ttu-id="7cc0c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cc0c-131">Type</span></span>|<span data-ttu-id="7cc0c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cc0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cc0c-133">id</span><span class="sxs-lookup"><span data-stu-id="7cc0c-133">id</span></span>|<span data-ttu-id="7cc0c-134">String</span><span class="sxs-lookup"><span data-stu-id="7cc0c-134">String</span></span>|<span data-ttu-id="7cc0c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-135">Key of the entity.</span></span> <span data-ttu-id="7cc0c-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="7cc0c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7cc0c-137">displayName</span></span>|<span data-ttu-id="7cc0c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cc0c-138">String</span></span>|<span data-ttu-id="7cc0c-139">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="7cc0c-140">descrição</span><span class="sxs-lookup"><span data-stu-id="7cc0c-140">description</span></span>|<span data-ttu-id="7cc0c-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cc0c-141">String</span></span>|<span data-ttu-id="7cc0c-142">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="7cc0c-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="7cc0c-143">scopeMembers</span></span>|<span data-ttu-id="7cc0c-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cc0c-144">String collection</span></span>|<span data-ttu-id="7cc0c-145">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="7cc0c-146">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="7cc0c-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="7cc0c-147">scopeType</span></span>|[<span data-ttu-id="7cc0c-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="7cc0c-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="7cc0c-149">Especifica o tipo de escopo para uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="7cc0c-150">O tipo de padrão 'ResourceScope' permite que a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="7cc0c-151">Para 'AllDevices', 'AllLicensedUsers' e 'AllDevicesAndLicensedUsers', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="7cc0c-152">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="7cc0c-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="7cc0c-153">resourceScopes</span></span>|<span data-ttu-id="7cc0c-154">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cc0c-154">String collection</span></span>|<span data-ttu-id="7cc0c-155">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="7cc0c-156">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="7cc0c-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cc0c-157">Response</span></span>
<span data-ttu-id="7cc0c-158">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-158">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cc0c-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cc0c-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cc0c-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cc0c-160">Request</span></span>
<span data-ttu-id="7cc0c-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="7cc0c-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cc0c-162">Response</span></span>
<span data-ttu-id="7cc0c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7cc0c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 326

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```





