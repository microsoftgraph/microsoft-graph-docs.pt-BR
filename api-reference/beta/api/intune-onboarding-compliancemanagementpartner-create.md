---
title: Criar complianceManagementPartner
description: Criar um novo objeto complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c1e1b41272304d4f9d6991f3bcc434f315d2b14f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791851"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="4b2b8-103">Criar complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="4b2b8-103">Create complianceManagementPartner</span></span>

<span data-ttu-id="4b2b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b2b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b2b8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b2b8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b2b8-107">Criar um novo objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="4b2b8-107">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b2b8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b2b8-108">Prerequisites</span></span>
<span data-ttu-id="4b2b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b2b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b2b8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b2b8-111">Permission type</span></span>|<span data-ttu-id="4b2b8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b2b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b2b8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b2b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b2b8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b2b8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4b2b8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b2b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b2b8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-116">Not supported.</span></span>|
|<span data-ttu-id="4b2b8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b2b8-117">Application</span></span>|<span data-ttu-id="4b2b8-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b2b8-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b2b8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b2b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="4b2b8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b2b8-120">Request headers</span></span>
|<span data-ttu-id="4b2b8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b2b8-121">Header</span></span>|<span data-ttu-id="4b2b8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4b2b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b2b8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b2b8-123">Authorization</span></span>|<span data-ttu-id="4b2b8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b2b8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b2b8-125">Accept</span></span>|<span data-ttu-id="4b2b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b2b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b2b8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b2b8-127">Request body</span></span>
<span data-ttu-id="4b2b8-128">No corpo da solicitação, forneça uma representação JSON do objeto complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-128">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="4b2b8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-129">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="4b2b8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b2b8-130">Property</span></span>|<span data-ttu-id="4b2b8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b2b8-131">Type</span></span>|<span data-ttu-id="4b2b8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b2b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b2b8-133">id</span><span class="sxs-lookup"><span data-stu-id="4b2b8-133">id</span></span>|<span data-ttu-id="4b2b8-134">String</span><span class="sxs-lookup"><span data-stu-id="4b2b8-134">String</span></span>|<span data-ttu-id="4b2b8-135">ID da entidade</span><span class="sxs-lookup"><span data-stu-id="4b2b8-135">Id of the entity</span></span>|
|<span data-ttu-id="4b2b8-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="4b2b8-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="4b2b8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b2b8-137">DateTimeOffset</span></span>|<span data-ttu-id="4b2b8-138">Carimbo de data/hora da última pulsação após o administrador integrado ao parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="4b2b8-138">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="4b2b8-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="4b2b8-139">partnerState</span></span>|[<span data-ttu-id="4b2b8-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="4b2b8-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="4b2b8-141">Estado do parceiro desse locatário.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-141">Partner state of this tenant.</span></span> <span data-ttu-id="4b2b8-142">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="4b2b8-143">displayName</span><span class="sxs-lookup"><span data-stu-id="4b2b8-143">displayName</span></span>|<span data-ttu-id="4b2b8-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b2b8-144">String</span></span>|<span data-ttu-id="4b2b8-145">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="4b2b8-145">Partner display name</span></span>|
|<span data-ttu-id="4b2b8-146">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="4b2b8-146">macOsOnboarded</span></span>|<span data-ttu-id="4b2b8-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b2b8-147">Boolean</span></span>|<span data-ttu-id="4b2b8-148">Parceiro integrado para dispositivos Mac.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-148">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="4b2b8-149">windowsOnboarded</span><span class="sxs-lookup"><span data-stu-id="4b2b8-149">windowsOnboarded</span></span>|<span data-ttu-id="4b2b8-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b2b8-150">Boolean</span></span>|<span data-ttu-id="4b2b8-151">Parceiro integrado para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-151">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="4b2b8-152">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="4b2b8-152">androidOnboarded</span></span>|<span data-ttu-id="4b2b8-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b2b8-153">Boolean</span></span>|<span data-ttu-id="4b2b8-154">Parceiro integrado para dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-154">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="4b2b8-155">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="4b2b8-155">iosOnboarded</span></span>|<span data-ttu-id="4b2b8-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b2b8-156">Boolean</span></span>|<span data-ttu-id="4b2b8-157">Parceiro integrado para dispositivos IOS.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-157">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="4b2b8-158">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="4b2b8-158">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="4b2b8-159">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4b2b8-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="4b2b8-160">Grupos de usuários que inscrevem dispositivos Mac por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-160">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="4b2b8-161">windowsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="4b2b8-161">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="4b2b8-162">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4b2b8-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="4b2b8-163">Grupos de usuários que registram dispositivos do Windows por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-163">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="4b2b8-164">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="4b2b8-164">androidEnrollmentAssignments</span></span>|<span data-ttu-id="4b2b8-165">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4b2b8-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="4b2b8-166">Grupos de usuários que registram dispositivos Android por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-166">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="4b2b8-167">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="4b2b8-167">iosEnrollmentAssignments</span></span>|<span data-ttu-id="4b2b8-168">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4b2b8-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="4b2b8-169">Grupos de usuários que registram dispositivos IOS por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-169">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="4b2b8-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b2b8-170">Response</span></span>
<span data-ttu-id="4b2b8-171">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-171">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b2b8-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b2b8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b2b8-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b2b8-173">Request</span></span>
<span data-ttu-id="4b2b8-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
Content-type: application/json
Content-length: 1944

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
  "windowsOnboarded": true,
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4b2b8-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b2b8-175">Response</span></span>
<span data-ttu-id="4b2b8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b2b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1993

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
  "windowsOnboarded": true,
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



