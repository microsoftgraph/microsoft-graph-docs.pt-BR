---
title: Atualizar roleAssignment
description: Atualizar as propriedades de um objeto roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e4b5cde12d464d2b92f9348445bb793e4114833b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852014"
---
# <a name="update-roleassignment"></a><span data-ttu-id="7c319-103">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="7c319-103">Update roleAssignment</span></span>

> <span data-ttu-id="7c319-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7c319-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c319-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7c319-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c319-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7c319-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c319-107">Atualizar as propriedades de um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7c319-107">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c319-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c319-108">Prerequisites</span></span>
<span data-ttu-id="7c319-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c319-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c319-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c319-111">Permission type</span></span>|<span data-ttu-id="7c319-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7c319-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c319-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c319-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c319-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c319-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="7c319-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c319-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c319-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c319-116">Not supported.</span></span>|
|<span data-ttu-id="7c319-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c319-117">Application</span></span>|<span data-ttu-id="7c319-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c319-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c319-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c319-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7c319-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c319-120">Request headers</span></span>
|<span data-ttu-id="7c319-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c319-121">Header</span></span>|<span data-ttu-id="7c319-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7c319-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c319-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c319-123">Authorization</span></span>|<span data-ttu-id="7c319-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c319-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c319-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c319-125">Accept</span></span>|<span data-ttu-id="7c319-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c319-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c319-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c319-127">Request body</span></span>
<span data-ttu-id="7c319-128">No corpo da solicitação, forneça uma representação JSON do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7c319-128">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="7c319-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7c319-129">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="7c319-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c319-130">Property</span></span>|<span data-ttu-id="7c319-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c319-131">Type</span></span>|<span data-ttu-id="7c319-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c319-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c319-133">id</span><span class="sxs-lookup"><span data-stu-id="7c319-133">id</span></span>|<span data-ttu-id="7c319-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c319-134">String</span></span>|<span data-ttu-id="7c319-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7c319-135">Key of the entity.</span></span> <span data-ttu-id="7c319-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="7c319-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="7c319-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7c319-137">displayName</span></span>|<span data-ttu-id="7c319-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c319-138">String</span></span>|<span data-ttu-id="7c319-139">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7c319-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="7c319-140">descrição</span><span class="sxs-lookup"><span data-stu-id="7c319-140">description</span></span>|<span data-ttu-id="7c319-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c319-141">String</span></span>|<span data-ttu-id="7c319-142">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7c319-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="7c319-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="7c319-143">scopeMembers</span></span>|<span data-ttu-id="7c319-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c319-144">String collection</span></span>|<span data-ttu-id="7c319-145">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="7c319-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="7c319-146">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7c319-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="7c319-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="7c319-147">scopeType</span></span>|[<span data-ttu-id="7c319-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="7c319-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="7c319-149">Especifica o tipo de escopo para uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7c319-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="7c319-150">O tipo de padrão 'ResourceScope' permite que a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="7c319-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="7c319-151">Para 'AllDevices', 'AllLicensedUsers' e 'AllDevicesAndLicensedUsers', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="7c319-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="7c319-152">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="7c319-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="7c319-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="7c319-153">resourceScopes</span></span>|<span data-ttu-id="7c319-154">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c319-154">String collection</span></span>|<span data-ttu-id="7c319-155">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="7c319-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="7c319-156">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7c319-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="7c319-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c319-157">Response</span></span>
<span data-ttu-id="7c319-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c319-158">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c319-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c319-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c319-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c319-160">Request</span></span>
<span data-ttu-id="7c319-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c319-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 224

{
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

### <a name="response"></a><span data-ttu-id="7c319-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c319-162">Response</span></span>
<span data-ttu-id="7c319-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c319-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





