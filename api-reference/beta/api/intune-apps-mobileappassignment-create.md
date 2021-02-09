---
title: Criar mobileAppAssignment
description: Criar um novo objeto mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: acbdf694aeb6a6db39f89d57b5a6e06d9206a440
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155381"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="ace73-103">Criar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="ace73-103">Create mobileAppAssignment</span></span>

<span data-ttu-id="ace73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ace73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ace73-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ace73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ace73-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ace73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ace73-107">Criar um novo objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ace73-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ace73-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ace73-108">Prerequisites</span></span>
<span data-ttu-id="ace73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ace73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ace73-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ace73-111">Permission type</span></span>|<span data-ttu-id="ace73-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ace73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ace73-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ace73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ace73-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ace73-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ace73-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ace73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ace73-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ace73-116">Not supported.</span></span>|
|<span data-ttu-id="ace73-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ace73-117">Application</span></span>|<span data-ttu-id="ace73-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ace73-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ace73-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ace73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ace73-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ace73-120">Request headers</span></span>
|<span data-ttu-id="ace73-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ace73-121">Header</span></span>|<span data-ttu-id="ace73-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ace73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ace73-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ace73-123">Authorization</span></span>|<span data-ttu-id="ace73-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ace73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ace73-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ace73-125">Accept</span></span>|<span data-ttu-id="ace73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ace73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ace73-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ace73-127">Request body</span></span>
<span data-ttu-id="ace73-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="ace73-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="ace73-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="ace73-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="ace73-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ace73-130">Property</span></span>|<span data-ttu-id="ace73-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ace73-131">Type</span></span>|<span data-ttu-id="ace73-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ace73-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ace73-133">id</span><span class="sxs-lookup"><span data-stu-id="ace73-133">id</span></span>|<span data-ttu-id="ace73-134">String</span><span class="sxs-lookup"><span data-stu-id="ace73-134">String</span></span>|<span data-ttu-id="ace73-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ace73-135">Key of the entity.</span></span>|
|<span data-ttu-id="ace73-136">finalidade</span><span class="sxs-lookup"><span data-stu-id="ace73-136">intent</span></span>|[<span data-ttu-id="ace73-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="ace73-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ace73-138">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ace73-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="ace73-139">destino</span><span class="sxs-lookup"><span data-stu-id="ace73-139">target</span></span>|[<span data-ttu-id="ace73-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ace73-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ace73-141">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ace73-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="ace73-142">configurações</span><span class="sxs-lookup"><span data-stu-id="ace73-142">settings</span></span>|[<span data-ttu-id="ace73-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ace73-143">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="ace73-144">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ace73-144">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="ace73-145">source</span><span class="sxs-lookup"><span data-stu-id="ace73-145">source</span></span>|[<span data-ttu-id="ace73-146">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="ace73-146">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="ace73-147">O tipo de recurso que é a origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ace73-147">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="ace73-148">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="ace73-148">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="ace73-149">sourceId</span><span class="sxs-lookup"><span data-stu-id="ace73-149">sourceId</span></span>|<span data-ttu-id="ace73-150">String</span><span class="sxs-lookup"><span data-stu-id="ace73-150">String</span></span>|<span data-ttu-id="ace73-151">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ace73-151">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="ace73-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="ace73-152">Response</span></span>
<span data-ttu-id="ace73-153">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ace73-153">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ace73-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ace73-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="ace73-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ace73-155">Request</span></span>
<span data-ttu-id="ace73-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ace73-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 617

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="ace73-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="ace73-157">Response</span></span>
<span data-ttu-id="ace73-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ace73-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 666

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




