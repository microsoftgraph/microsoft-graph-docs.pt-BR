---
title: Criar roleAssignment
description: Criar um novo objeto roleAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8a8c889e401664fb0fea66030ff3bcabd0631503
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399910"
---
# <a name="create-roleassignment"></a><span data-ttu-id="0e91a-103">Criar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="0e91a-103">Create roleAssignment</span></span>

> <span data-ttu-id="0e91a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0e91a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0e91a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0e91a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e91a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0e91a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e91a-107">Criar um novo objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0e91a-107">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e91a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e91a-108">Prerequisites</span></span>
<span data-ttu-id="0e91a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0e91a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0e91a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e91a-111">Permission type</span></span>|<span data-ttu-id="0e91a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0e91a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e91a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e91a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e91a-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e91a-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0e91a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e91a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e91a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e91a-116">Not supported.</span></span>|
|<span data-ttu-id="0e91a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e91a-117">Application</span></span>|<span data-ttu-id="0e91a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e91a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e91a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e91a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="0e91a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e91a-120">Request headers</span></span>
|<span data-ttu-id="0e91a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e91a-121">Header</span></span>|<span data-ttu-id="0e91a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0e91a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e91a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e91a-123">Authorization</span></span>|<span data-ttu-id="0e91a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e91a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e91a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e91a-125">Accept</span></span>|<span data-ttu-id="0e91a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e91a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e91a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e91a-127">Request body</span></span>
<span data-ttu-id="0e91a-128">No corpo da solicitação, forneça uma representação JSON do objeto roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="0e91a-128">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="0e91a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="0e91a-129">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="0e91a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e91a-130">Property</span></span>|<span data-ttu-id="0e91a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e91a-131">Type</span></span>|<span data-ttu-id="0e91a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e91a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e91a-133">id</span><span class="sxs-lookup"><span data-stu-id="0e91a-133">id</span></span>|<span data-ttu-id="0e91a-134">String</span><span class="sxs-lookup"><span data-stu-id="0e91a-134">String</span></span>|<span data-ttu-id="0e91a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0e91a-135">Key of the entity.</span></span> <span data-ttu-id="0e91a-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="0e91a-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="0e91a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0e91a-137">displayName</span></span>|<span data-ttu-id="0e91a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e91a-138">String</span></span>|<span data-ttu-id="0e91a-139">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="0e91a-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="0e91a-140">descrição</span><span class="sxs-lookup"><span data-stu-id="0e91a-140">description</span></span>|<span data-ttu-id="0e91a-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e91a-141">String</span></span>|<span data-ttu-id="0e91a-142">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="0e91a-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="0e91a-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="0e91a-143">scopeMembers</span></span>|<span data-ttu-id="0e91a-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e91a-144">String collection</span></span>|<span data-ttu-id="0e91a-145">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="0e91a-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="0e91a-146">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0e91a-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="0e91a-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="0e91a-147">scopeType</span></span>|[<span data-ttu-id="0e91a-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="0e91a-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="0e91a-149">Especifica o tipo de escopo para uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="0e91a-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="0e91a-150">O tipo de padrão 'ResourceScope' permite que a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="0e91a-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="0e91a-151">Para 'AllDevices', 'AllLicensedUsers' e 'AllDevicesAndLicensedUsers', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="0e91a-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="0e91a-152">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="0e91a-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="0e91a-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="0e91a-153">resourceScopes</span></span>|<span data-ttu-id="0e91a-154">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e91a-154">String collection</span></span>|<span data-ttu-id="0e91a-155">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="0e91a-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="0e91a-156">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0e91a-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="0e91a-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e91a-157">Response</span></span>
<span data-ttu-id="0e91a-158">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e91a-158">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e91a-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e91a-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e91a-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e91a-160">Request</span></span>
<span data-ttu-id="0e91a-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e91a-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e91a-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e91a-162">Response</span></span>
<span data-ttu-id="0e91a-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e91a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




