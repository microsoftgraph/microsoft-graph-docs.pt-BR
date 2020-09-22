---
title: Atualizar roleAssignment
description: Atualizar as propriedades de um objeto roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d9acf221b7cf1e799679edb913de80cfd20d4a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056006"
---
# <a name="update-roleassignment"></a><span data-ttu-id="c0b60-103">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="c0b60-103">Update roleAssignment</span></span>

<span data-ttu-id="c0b60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0b60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0b60-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0b60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0b60-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0b60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0b60-107">Atualizar as propriedades de um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0b60-107">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0b60-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0b60-108">Prerequisites</span></span>
<span data-ttu-id="c0b60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0b60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0b60-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0b60-111">Permission type</span></span>|<span data-ttu-id="c0b60-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0b60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0b60-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0b60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0b60-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0b60-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c0b60-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0b60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0b60-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0b60-116">Not supported.</span></span>|
|<span data-ttu-id="c0b60-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0b60-117">Application</span></span>|<span data-ttu-id="c0b60-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0b60-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0b60-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0b60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c0b60-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0b60-120">Request headers</span></span>
|<span data-ttu-id="c0b60-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0b60-121">Header</span></span>|<span data-ttu-id="c0b60-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c0b60-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0b60-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0b60-123">Authorization</span></span>|<span data-ttu-id="c0b60-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0b60-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0b60-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0b60-125">Accept</span></span>|<span data-ttu-id="c0b60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0b60-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0b60-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0b60-127">Request body</span></span>
<span data-ttu-id="c0b60-128">No corpo da solicitação, forneça uma representação JSON do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0b60-128">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="c0b60-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0b60-129">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="c0b60-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0b60-130">Property</span></span>|<span data-ttu-id="c0b60-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0b60-131">Type</span></span>|<span data-ttu-id="c0b60-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0b60-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0b60-133">id</span><span class="sxs-lookup"><span data-stu-id="c0b60-133">id</span></span>|<span data-ttu-id="c0b60-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0b60-134">String</span></span>|<span data-ttu-id="c0b60-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c0b60-135">Key of the entity.</span></span> <span data-ttu-id="c0b60-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="c0b60-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="c0b60-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c0b60-137">displayName</span></span>|<span data-ttu-id="c0b60-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0b60-138">String</span></span>|<span data-ttu-id="c0b60-139">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c0b60-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="c0b60-140">description</span><span class="sxs-lookup"><span data-stu-id="c0b60-140">description</span></span>|<span data-ttu-id="c0b60-141">String</span><span class="sxs-lookup"><span data-stu-id="c0b60-141">String</span></span>|<span data-ttu-id="c0b60-142">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c0b60-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="c0b60-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="c0b60-143">scopeMembers</span></span>|<span data-ttu-id="c0b60-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0b60-144">String collection</span></span>|<span data-ttu-id="c0b60-145">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="c0b60-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="c0b60-146">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c0b60-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="c0b60-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="c0b60-147">scopeType</span></span>|[<span data-ttu-id="c0b60-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="c0b60-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="c0b60-149">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c0b60-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="c0b60-150">O tipo padrão ' ResourceScope ' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="c0b60-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="c0b60-151">Para ' mydevices ', ' AllLicensedUsers ' e ' AllDevicesAndLicensedUsers ', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="c0b60-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="c0b60-152">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="c0b60-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="c0b60-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="c0b60-153">resourceScopes</span></span>|<span data-ttu-id="c0b60-154">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0b60-154">String collection</span></span>|<span data-ttu-id="c0b60-155">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="c0b60-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="c0b60-156">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c0b60-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="c0b60-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0b60-157">Response</span></span>
<span data-ttu-id="c0b60-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0b60-158">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0b60-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0b60-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0b60-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0b60-160">Request</span></span>
<span data-ttu-id="c0b60-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0b60-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
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

### <a name="response"></a><span data-ttu-id="c0b60-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0b60-162">Response</span></span>
<span data-ttu-id="c0b60-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0b60-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






