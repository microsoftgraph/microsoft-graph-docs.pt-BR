---
title: Atualizar roleAssignment
description: Atualizar as propriedades de um objeto roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f35f7ee957250a546d721a615036f18648d28ff7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913869"
---
# <a name="update-roleassignment"></a><span data-ttu-id="44ad7-103">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="44ad7-103">Update roleAssignment</span></span>

> <span data-ttu-id="44ad7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="44ad7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44ad7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="44ad7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44ad7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="44ad7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44ad7-107">Atualizar as propriedades de um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="44ad7-107">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44ad7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44ad7-108">Prerequisites</span></span>
<span data-ttu-id="44ad7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44ad7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44ad7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44ad7-111">Permission type</span></span>|<span data-ttu-id="44ad7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="44ad7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44ad7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44ad7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44ad7-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44ad7-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="44ad7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44ad7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44ad7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44ad7-116">Not supported.</span></span>|
|<span data-ttu-id="44ad7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44ad7-117">Application</span></span>|<span data-ttu-id="44ad7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44ad7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44ad7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44ad7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="44ad7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44ad7-120">Request headers</span></span>
|<span data-ttu-id="44ad7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44ad7-121">Header</span></span>|<span data-ttu-id="44ad7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="44ad7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44ad7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="44ad7-123">Authorization</span></span>|<span data-ttu-id="44ad7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44ad7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44ad7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="44ad7-125">Accept</span></span>|<span data-ttu-id="44ad7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44ad7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44ad7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44ad7-127">Request body</span></span>
<span data-ttu-id="44ad7-128">No corpo da solicitação, forneça uma representação JSON do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="44ad7-128">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="44ad7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="44ad7-129">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="44ad7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44ad7-130">Property</span></span>|<span data-ttu-id="44ad7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="44ad7-131">Type</span></span>|<span data-ttu-id="44ad7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="44ad7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ad7-133">id</span><span class="sxs-lookup"><span data-stu-id="44ad7-133">id</span></span>|<span data-ttu-id="44ad7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44ad7-134">String</span></span>|<span data-ttu-id="44ad7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="44ad7-135">Key of the entity.</span></span> <span data-ttu-id="44ad7-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="44ad7-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="44ad7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="44ad7-137">displayName</span></span>|<span data-ttu-id="44ad7-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44ad7-138">String</span></span>|<span data-ttu-id="44ad7-139">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="44ad7-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="44ad7-140">descrição</span><span class="sxs-lookup"><span data-stu-id="44ad7-140">description</span></span>|<span data-ttu-id="44ad7-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44ad7-141">String</span></span>|<span data-ttu-id="44ad7-142">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="44ad7-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="44ad7-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="44ad7-143">scopeMembers</span></span>|<span data-ttu-id="44ad7-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="44ad7-144">String collection</span></span>|<span data-ttu-id="44ad7-145">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="44ad7-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="44ad7-146">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="44ad7-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="44ad7-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="44ad7-147">scopeType</span></span>|[<span data-ttu-id="44ad7-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="44ad7-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="44ad7-149">Especifica o tipo de escopo para uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="44ad7-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="44ad7-150">O tipo de padrão 'ResourceScope' permite que a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="44ad7-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="44ad7-151">Para 'AllDevices', 'AllLicensedUsers' e 'AllDevicesAndLicensedUsers', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="44ad7-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="44ad7-152">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="44ad7-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="44ad7-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="44ad7-153">resourceScopes</span></span>|<span data-ttu-id="44ad7-154">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="44ad7-154">String collection</span></span>|<span data-ttu-id="44ad7-155">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="44ad7-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="44ad7-156">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="44ad7-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="44ad7-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="44ad7-157">Response</span></span>
<span data-ttu-id="44ad7-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44ad7-158">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44ad7-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44ad7-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="44ad7-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44ad7-160">Request</span></span>
<span data-ttu-id="44ad7-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44ad7-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44ad7-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="44ad7-162">Response</span></span>
<span data-ttu-id="44ad7-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44ad7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





