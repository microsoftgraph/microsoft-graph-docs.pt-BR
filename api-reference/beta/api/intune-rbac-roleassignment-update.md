---
title: Atualizar roleAssignment
description: Atualizar as propriedades de um objeto roleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 82bf64be5658606166bad9de48c1f44a2c68a73e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459692"
---
# <a name="update-roleassignment"></a><span data-ttu-id="d1d93-103">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d1d93-103">Update roleAssignment</span></span>

<span data-ttu-id="d1d93-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d1d93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1d93-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d1d93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1d93-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1d93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1d93-107">Atualizar as propriedades de um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d1d93-107">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1d93-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1d93-108">Prerequisites</span></span>
<span data-ttu-id="d1d93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1d93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1d93-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1d93-111">Permission type</span></span>|<span data-ttu-id="d1d93-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1d93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1d93-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1d93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1d93-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1d93-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d1d93-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1d93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1d93-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1d93-116">Not supported.</span></span>|
|<span data-ttu-id="d1d93-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1d93-117">Application</span></span>|<span data-ttu-id="d1d93-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1d93-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1d93-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1d93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d1d93-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1d93-120">Request headers</span></span>
|<span data-ttu-id="d1d93-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1d93-121">Header</span></span>|<span data-ttu-id="d1d93-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d1d93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1d93-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1d93-123">Authorization</span></span>|<span data-ttu-id="d1d93-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1d93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1d93-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1d93-125">Accept</span></span>|<span data-ttu-id="d1d93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1d93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1d93-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1d93-127">Request body</span></span>
<span data-ttu-id="d1d93-128">No corpo da solicitação, forneça uma representação JSON do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d1d93-128">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="d1d93-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d1d93-129">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="d1d93-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1d93-130">Property</span></span>|<span data-ttu-id="d1d93-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1d93-131">Type</span></span>|<span data-ttu-id="d1d93-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1d93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1d93-133">id</span><span class="sxs-lookup"><span data-stu-id="d1d93-133">id</span></span>|<span data-ttu-id="d1d93-134">String</span><span class="sxs-lookup"><span data-stu-id="d1d93-134">String</span></span>|<span data-ttu-id="d1d93-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d1d93-135">Key of the entity.</span></span> <span data-ttu-id="d1d93-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d1d93-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="d1d93-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d1d93-137">displayName</span></span>|<span data-ttu-id="d1d93-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1d93-138">String</span></span>|<span data-ttu-id="d1d93-139">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d1d93-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="d1d93-140">description</span><span class="sxs-lookup"><span data-stu-id="d1d93-140">description</span></span>|<span data-ttu-id="d1d93-141">String</span><span class="sxs-lookup"><span data-stu-id="d1d93-141">String</span></span>|<span data-ttu-id="d1d93-142">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d1d93-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="d1d93-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="d1d93-143">scopeMembers</span></span>|<span data-ttu-id="d1d93-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1d93-144">String collection</span></span>|<span data-ttu-id="d1d93-145">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="d1d93-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="d1d93-146">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d1d93-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="d1d93-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="d1d93-147">scopeType</span></span>|[<span data-ttu-id="d1d93-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="d1d93-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="d1d93-149">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d1d93-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="d1d93-150">O tipo padrão ' ResourceScope ' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="d1d93-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="d1d93-151">Para ' mydevices ', ' AllLicensedUsers ' e ' AllDevicesAndLicensedUsers ', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="d1d93-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="d1d93-152">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="d1d93-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="d1d93-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="d1d93-153">resourceScopes</span></span>|<span data-ttu-id="d1d93-154">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1d93-154">String collection</span></span>|<span data-ttu-id="d1d93-155">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="d1d93-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="d1d93-156">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d1d93-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="d1d93-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1d93-157">Response</span></span>
<span data-ttu-id="d1d93-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1d93-158">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1d93-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1d93-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1d93-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1d93-160">Request</span></span>
<span data-ttu-id="d1d93-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1d93-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d1d93-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1d93-162">Response</span></span>
<span data-ttu-id="d1d93-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1d93-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





