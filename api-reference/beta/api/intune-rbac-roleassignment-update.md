---
title: Atualizar roleAssignment
description: Atualizar as propriedades de um objeto roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ccb927a4a1ac2f02264db1ac81e814c4b5aa1abe
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141593"
---
# <a name="update-roleassignment"></a><span data-ttu-id="cb189-103">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="cb189-103">Update roleAssignment</span></span>

<span data-ttu-id="cb189-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb189-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb189-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb189-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb189-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb189-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb189-107">Atualizar as propriedades de um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cb189-107">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb189-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb189-108">Prerequisites</span></span>
<span data-ttu-id="cb189-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb189-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb189-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb189-111">Permission type</span></span>|<span data-ttu-id="cb189-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb189-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb189-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb189-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb189-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb189-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="cb189-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb189-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb189-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb189-116">Not supported.</span></span>|
|<span data-ttu-id="cb189-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb189-117">Application</span></span>|<span data-ttu-id="cb189-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb189-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb189-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb189-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="cb189-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb189-120">Request headers</span></span>
|<span data-ttu-id="cb189-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb189-121">Header</span></span>|<span data-ttu-id="cb189-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cb189-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb189-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb189-123">Authorization</span></span>|<span data-ttu-id="cb189-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb189-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb189-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cb189-125">Accept</span></span>|<span data-ttu-id="cb189-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb189-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb189-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb189-127">Request body</span></span>
<span data-ttu-id="cb189-128">No corpo da solicitação, forneça uma representação JSON do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cb189-128">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="cb189-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cb189-129">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="cb189-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb189-130">Property</span></span>|<span data-ttu-id="cb189-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb189-131">Type</span></span>|<span data-ttu-id="cb189-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb189-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb189-133">id</span><span class="sxs-lookup"><span data-stu-id="cb189-133">id</span></span>|<span data-ttu-id="cb189-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb189-134">String</span></span>|<span data-ttu-id="cb189-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cb189-135">Key of the entity.</span></span> <span data-ttu-id="cb189-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="cb189-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="cb189-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cb189-137">displayName</span></span>|<span data-ttu-id="cb189-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb189-138">String</span></span>|<span data-ttu-id="cb189-139">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="cb189-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="cb189-140">descrição</span><span class="sxs-lookup"><span data-stu-id="cb189-140">description</span></span>|<span data-ttu-id="cb189-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb189-141">String</span></span>|<span data-ttu-id="cb189-142">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="cb189-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="cb189-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="cb189-143">scopeMembers</span></span>|<span data-ttu-id="cb189-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb189-144">String collection</span></span>|<span data-ttu-id="cb189-145">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="cb189-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="cb189-146">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cb189-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="cb189-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="cb189-147">scopeType</span></span>|[<span data-ttu-id="cb189-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="cb189-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="cb189-149">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="cb189-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="cb189-150">O tipo padrão 'ResourceScope' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="cb189-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="cb189-151">Para 'AllDevices', 'AllLicensedUsers' e 'AllDevicesAndLicensedUsers', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="cb189-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="cb189-152">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="cb189-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="cb189-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="cb189-153">resourceScopes</span></span>|<span data-ttu-id="cb189-154">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb189-154">String collection</span></span>|<span data-ttu-id="cb189-155">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="cb189-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="cb189-156">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cb189-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="cb189-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb189-157">Response</span></span>
<span data-ttu-id="cb189-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb189-158">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb189-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb189-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb189-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb189-160">Request</span></span>
<span data-ttu-id="cb189-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb189-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cb189-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb189-162">Response</span></span>
<span data-ttu-id="cb189-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb189-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




