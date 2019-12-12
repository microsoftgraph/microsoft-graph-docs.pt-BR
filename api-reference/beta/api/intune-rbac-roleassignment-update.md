---
title: Atualizar roleAssignment
description: Atualizar as propriedades de um objeto roleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b28793cd9e484934e97f7b78e91f5568e8b347a8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955270"
---
# <a name="update-roleassignment"></a><span data-ttu-id="128b4-103">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="128b4-103">Update roleAssignment</span></span>

> <span data-ttu-id="128b4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="128b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="128b4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="128b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="128b4-106">Atualizar as propriedades de um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="128b4-106">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="128b4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="128b4-107">Prerequisites</span></span>
<span data-ttu-id="128b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="128b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="128b4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="128b4-110">Permission type</span></span>|<span data-ttu-id="128b4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="128b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="128b4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="128b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="128b4-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="128b4-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="128b4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="128b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="128b4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="128b4-115">Not supported.</span></span>|
|<span data-ttu-id="128b4-116">Application</span><span class="sxs-lookup"><span data-stu-id="128b4-116">Application</span></span>|<span data-ttu-id="128b4-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="128b4-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="128b4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="128b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="128b4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="128b4-119">Request headers</span></span>
|<span data-ttu-id="128b4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="128b4-120">Header</span></span>|<span data-ttu-id="128b4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="128b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="128b4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="128b4-122">Authorization</span></span>|<span data-ttu-id="128b4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="128b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="128b4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="128b4-124">Accept</span></span>|<span data-ttu-id="128b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="128b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="128b4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="128b4-126">Request body</span></span>
<span data-ttu-id="128b4-127">No corpo da solicitação, forneça uma representação JSON do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="128b4-127">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="128b4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="128b4-128">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="128b4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="128b4-129">Property</span></span>|<span data-ttu-id="128b4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="128b4-130">Type</span></span>|<span data-ttu-id="128b4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="128b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="128b4-132">id</span><span class="sxs-lookup"><span data-stu-id="128b4-132">id</span></span>|<span data-ttu-id="128b4-133">String</span><span class="sxs-lookup"><span data-stu-id="128b4-133">String</span></span>|<span data-ttu-id="128b4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="128b4-134">Key of the entity.</span></span> <span data-ttu-id="128b4-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="128b4-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="128b4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="128b4-136">displayName</span></span>|<span data-ttu-id="128b4-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="128b4-137">String</span></span>|<span data-ttu-id="128b4-138">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="128b4-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="128b4-139">description</span><span class="sxs-lookup"><span data-stu-id="128b4-139">description</span></span>|<span data-ttu-id="128b4-140">String</span><span class="sxs-lookup"><span data-stu-id="128b4-140">String</span></span>|<span data-ttu-id="128b4-141">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="128b4-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="128b4-142">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="128b4-142">scopeMembers</span></span>|<span data-ttu-id="128b4-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="128b4-143">String collection</span></span>|<span data-ttu-id="128b4-144">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="128b4-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="128b4-145">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="128b4-145">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="128b4-146">scopeType</span><span class="sxs-lookup"><span data-stu-id="128b4-146">scopeType</span></span>|[<span data-ttu-id="128b4-147">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="128b4-147">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="128b4-148">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="128b4-148">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="128b4-149">O tipo padrão ' ResourceScope ' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="128b4-149">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="128b4-150">Para ' mydevices ', ' AllLicensedUsers ' e ' AllDevicesAndLicensedUsers ', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="128b4-150">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="128b4-151">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="128b4-151">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="128b4-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="128b4-152">resourceScopes</span></span>|<span data-ttu-id="128b4-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="128b4-153">String collection</span></span>|<span data-ttu-id="128b4-154">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="128b4-154">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="128b4-155">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="128b4-155">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="128b4-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="128b4-156">Response</span></span>
<span data-ttu-id="128b4-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="128b4-157">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="128b4-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="128b4-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="128b4-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="128b4-159">Request</span></span>
<span data-ttu-id="128b4-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="128b4-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="128b4-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="128b4-161">Response</span></span>
<span data-ttu-id="128b4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="128b4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





