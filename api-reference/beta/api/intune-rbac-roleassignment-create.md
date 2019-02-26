---
title: Criar roleAssignment
description: Criar um novo objeto roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7bbd3624649fc576c29afaf07c532fb627d83261
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161457"
---
# <a name="create-roleassignment"></a><span data-ttu-id="a0cd1-103">Criar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a0cd1-103">Create roleAssignment</span></span>

> <span data-ttu-id="a0cd1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0cd1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0cd1-106">Criar um novo objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a0cd1-106">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0cd1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0cd1-107">Prerequisites</span></span>
<span data-ttu-id="a0cd1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a0cd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a0cd1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0cd1-110">Permission type</span></span>|<span data-ttu-id="a0cd1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0cd1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0cd1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0cd1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0cd1-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0cd1-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="a0cd1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0cd1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0cd1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-115">Not supported.</span></span>|
|<span data-ttu-id="a0cd1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0cd1-116">Application</span></span>|<span data-ttu-id="a0cd1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0cd1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0cd1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a0cd1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0cd1-119">Request headers</span></span>
|<span data-ttu-id="a0cd1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0cd1-120">Header</span></span>|<span data-ttu-id="a0cd1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a0cd1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0cd1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0cd1-122">Authorization</span></span>|<span data-ttu-id="a0cd1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0cd1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0cd1-124">Accept</span></span>|<span data-ttu-id="a0cd1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0cd1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0cd1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0cd1-126">Request body</span></span>
<span data-ttu-id="a0cd1-127">No corpo da solicitação, forneça uma representação JSON do objeto roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-127">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="a0cd1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-128">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="a0cd1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0cd1-129">Property</span></span>|<span data-ttu-id="a0cd1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0cd1-130">Type</span></span>|<span data-ttu-id="a0cd1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0cd1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0cd1-132">id</span><span class="sxs-lookup"><span data-stu-id="a0cd1-132">id</span></span>|<span data-ttu-id="a0cd1-133">String</span><span class="sxs-lookup"><span data-stu-id="a0cd1-133">String</span></span>|<span data-ttu-id="a0cd1-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-134">Key of the entity.</span></span> <span data-ttu-id="a0cd1-135">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a0cd1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a0cd1-136">displayName</span></span>|<span data-ttu-id="a0cd1-137">String</span><span class="sxs-lookup"><span data-stu-id="a0cd1-137">String</span></span>|<span data-ttu-id="a0cd1-138">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="a0cd1-139">descrição</span><span class="sxs-lookup"><span data-stu-id="a0cd1-139">description</span></span>|<span data-ttu-id="a0cd1-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0cd1-140">String</span></span>|<span data-ttu-id="a0cd1-141">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="a0cd1-142">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="a0cd1-142">scopeMembers</span></span>|<span data-ttu-id="a0cd1-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0cd1-143">String collection</span></span>|<span data-ttu-id="a0cd1-144">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="a0cd1-145">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-145">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="a0cd1-146">scopeType</span><span class="sxs-lookup"><span data-stu-id="a0cd1-146">scopeType</span></span>|[<span data-ttu-id="a0cd1-147">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="a0cd1-147">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="a0cd1-148">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-148">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="a0cd1-149">O tipo padrão ' ResourceScope ' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-149">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="a0cd1-150">Para ' myDevices ', ' AllLicensedUsers ' e ' AllDevicesAndLicensedUsers ', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-150">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="a0cd1-151">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-151">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="a0cd1-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="a0cd1-152">resourceScopes</span></span>|<span data-ttu-id="a0cd1-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0cd1-153">String collection</span></span>|<span data-ttu-id="a0cd1-154">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-154">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="a0cd1-155">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-155">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="a0cd1-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0cd1-156">Response</span></span>
<span data-ttu-id="a0cd1-157">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-157">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0cd1-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0cd1-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0cd1-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0cd1-159">Request</span></span>
<span data-ttu-id="a0cd1-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0cd1-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0cd1-161">Response</span></span>
<span data-ttu-id="a0cd1-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0cd1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




