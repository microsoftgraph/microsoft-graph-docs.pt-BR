---
title: Criar mobileAppAssignment
description: Criar um novo objeto mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db319c40fd4f3150cf5f113d54ff3c7dd98731b3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977590"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="b4eeb-103">Criar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="b4eeb-103">Create mobileAppAssignment</span></span>

<span data-ttu-id="b4eeb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4eeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4eeb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4eeb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4eeb-107">Criar um novo objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b4eeb-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4eeb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4eeb-108">Prerequisites</span></span>
<span data-ttu-id="b4eeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4eeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4eeb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4eeb-111">Permission type</span></span>|<span data-ttu-id="b4eeb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4eeb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4eeb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4eeb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4eeb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4eeb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4eeb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4eeb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4eeb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-116">Not supported.</span></span>|
|<span data-ttu-id="b4eeb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4eeb-117">Application</span></span>|<span data-ttu-id="b4eeb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4eeb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4eeb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4eeb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b4eeb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4eeb-120">Request headers</span></span>
|<span data-ttu-id="b4eeb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4eeb-121">Header</span></span>|<span data-ttu-id="b4eeb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b4eeb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4eeb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4eeb-123">Authorization</span></span>|<span data-ttu-id="b4eeb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4eeb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4eeb-125">Accept</span></span>|<span data-ttu-id="b4eeb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4eeb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4eeb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4eeb-127">Request body</span></span>
<span data-ttu-id="b4eeb-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="b4eeb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="b4eeb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4eeb-130">Property</span></span>|<span data-ttu-id="b4eeb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4eeb-131">Type</span></span>|<span data-ttu-id="b4eeb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4eeb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4eeb-133">id</span><span class="sxs-lookup"><span data-stu-id="b4eeb-133">id</span></span>|<span data-ttu-id="b4eeb-134">String</span><span class="sxs-lookup"><span data-stu-id="b4eeb-134">String</span></span>|<span data-ttu-id="b4eeb-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-135">Key of the entity.</span></span>|
|<span data-ttu-id="b4eeb-136">finalidade</span><span class="sxs-lookup"><span data-stu-id="b4eeb-136">intent</span></span>|[<span data-ttu-id="b4eeb-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="b4eeb-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="b4eeb-138">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="b4eeb-139">destino</span><span class="sxs-lookup"><span data-stu-id="b4eeb-139">target</span></span>|[<span data-ttu-id="b4eeb-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b4eeb-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b4eeb-141">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="b4eeb-142">configurações</span><span class="sxs-lookup"><span data-stu-id="b4eeb-142">settings</span></span>|[<span data-ttu-id="b4eeb-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="b4eeb-143">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="b4eeb-144">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-144">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="b4eeb-145">source</span><span class="sxs-lookup"><span data-stu-id="b4eeb-145">source</span></span>|[<span data-ttu-id="b4eeb-146">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="b4eeb-146">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="b4eeb-147">O tipo de recurso que é a origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-147">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="b4eeb-148">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-148">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="b4eeb-149">sourceId</span><span class="sxs-lookup"><span data-stu-id="b4eeb-149">sourceId</span></span>|<span data-ttu-id="b4eeb-150">String</span><span class="sxs-lookup"><span data-stu-id="b4eeb-150">String</span></span>|<span data-ttu-id="b4eeb-151">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-151">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="b4eeb-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4eeb-152">Response</span></span>
<span data-ttu-id="b4eeb-153">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-153">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4eeb-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4eeb-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4eeb-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4eeb-155">Request</span></span>
<span data-ttu-id="b4eeb-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4eeb-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4eeb-157">Response</span></span>
<span data-ttu-id="b4eeb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4eeb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






