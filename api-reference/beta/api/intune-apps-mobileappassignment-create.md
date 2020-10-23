---
title: Criar mobileAppAssignment
description: Criar um novo objeto mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d72b4e21881b0813f0ac4808b8052df6072df9c5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699048"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="7fdba-103">Criar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="7fdba-103">Create mobileAppAssignment</span></span>

<span data-ttu-id="7fdba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fdba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7fdba-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7fdba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fdba-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7fdba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fdba-107">Criar um novo objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7fdba-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fdba-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7fdba-108">Prerequisites</span></span>
<span data-ttu-id="7fdba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fdba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fdba-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fdba-111">Permission type</span></span>|<span data-ttu-id="7fdba-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7fdba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fdba-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fdba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7fdba-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fdba-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7fdba-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fdba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fdba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fdba-116">Not supported.</span></span>|
|<span data-ttu-id="7fdba-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fdba-117">Application</span></span>|<span data-ttu-id="7fdba-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fdba-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fdba-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fdba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7fdba-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fdba-120">Request headers</span></span>
|<span data-ttu-id="7fdba-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7fdba-121">Header</span></span>|<span data-ttu-id="7fdba-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7fdba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fdba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fdba-123">Authorization</span></span>|<span data-ttu-id="7fdba-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fdba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fdba-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7fdba-125">Accept</span></span>|<span data-ttu-id="7fdba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7fdba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fdba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fdba-127">Request body</span></span>
<span data-ttu-id="7fdba-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="7fdba-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="7fdba-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="7fdba-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="7fdba-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7fdba-130">Property</span></span>|<span data-ttu-id="7fdba-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fdba-131">Type</span></span>|<span data-ttu-id="7fdba-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fdba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fdba-133">id</span><span class="sxs-lookup"><span data-stu-id="7fdba-133">id</span></span>|<span data-ttu-id="7fdba-134">String</span><span class="sxs-lookup"><span data-stu-id="7fdba-134">String</span></span>|<span data-ttu-id="7fdba-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7fdba-135">Key of the entity.</span></span>|
|<span data-ttu-id="7fdba-136">finalidade</span><span class="sxs-lookup"><span data-stu-id="7fdba-136">intent</span></span>|[<span data-ttu-id="7fdba-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="7fdba-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="7fdba-138">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="7fdba-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="7fdba-139">destino</span><span class="sxs-lookup"><span data-stu-id="7fdba-139">target</span></span>|[<span data-ttu-id="7fdba-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7fdba-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7fdba-141">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="7fdba-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="7fdba-142">configurações</span><span class="sxs-lookup"><span data-stu-id="7fdba-142">settings</span></span>|[<span data-ttu-id="7fdba-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="7fdba-143">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="7fdba-144">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="7fdba-144">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="7fdba-145">source</span><span class="sxs-lookup"><span data-stu-id="7fdba-145">source</span></span>|[<span data-ttu-id="7fdba-146">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="7fdba-146">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="7fdba-147">O tipo de recurso que é a origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="7fdba-147">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="7fdba-148">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="7fdba-148">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="7fdba-149">sourceId</span><span class="sxs-lookup"><span data-stu-id="7fdba-149">sourceId</span></span>|<span data-ttu-id="7fdba-150">String</span><span class="sxs-lookup"><span data-stu-id="7fdba-150">String</span></span>|<span data-ttu-id="7fdba-151">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="7fdba-151">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="7fdba-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fdba-152">Response</span></span>
<span data-ttu-id="7fdba-153">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fdba-153">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fdba-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fdba-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fdba-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fdba-155">Request</span></span>
<span data-ttu-id="7fdba-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fdba-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 591

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
    "uninstallOnDeviceRemoval": true
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="7fdba-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fdba-157">Response</span></span>
<span data-ttu-id="7fdba-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fdba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 640

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
    "uninstallOnDeviceRemoval": true
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```





