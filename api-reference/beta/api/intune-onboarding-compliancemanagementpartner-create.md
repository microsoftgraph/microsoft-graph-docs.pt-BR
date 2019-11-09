---
title: Criar complianceManagementPartner
description: Criar um novo objeto complianceManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d051fcd8ee5a86df62ee618b1ac871ac9ee81d3f
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086708"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="c6675-103">Criar complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="c6675-103">Create complianceManagementPartner</span></span>

> <span data-ttu-id="c6675-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6675-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6675-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6675-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6675-106">Criar um novo objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="c6675-106">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6675-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6675-107">Prerequisites</span></span>
<span data-ttu-id="c6675-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6675-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6675-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6675-110">Permission type</span></span>|<span data-ttu-id="c6675-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c6675-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6675-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6675-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6675-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6675-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c6675-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6675-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6675-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6675-115">Not supported.</span></span>|
|<span data-ttu-id="c6675-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6675-116">Application</span></span>|<span data-ttu-id="c6675-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6675-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6675-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6675-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="c6675-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6675-119">Request headers</span></span>
|<span data-ttu-id="c6675-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6675-120">Header</span></span>|<span data-ttu-id="c6675-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c6675-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6675-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6675-122">Authorization</span></span>|<span data-ttu-id="c6675-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6675-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6675-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c6675-124">Accept</span></span>|<span data-ttu-id="c6675-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6675-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6675-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6675-126">Request body</span></span>
<span data-ttu-id="c6675-127">No corpo da solicitação, forneça uma representação JSON do objeto complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="c6675-127">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="c6675-128">A tabela a seguir mostra as propriedades que são necessárias ao criar complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="c6675-128">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="c6675-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6675-129">Property</span></span>|<span data-ttu-id="c6675-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6675-130">Type</span></span>|<span data-ttu-id="c6675-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6675-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6675-132">id</span><span class="sxs-lookup"><span data-stu-id="c6675-132">id</span></span>|<span data-ttu-id="c6675-133">String</span><span class="sxs-lookup"><span data-stu-id="c6675-133">String</span></span>|<span data-ttu-id="c6675-134">ID da entidade</span><span class="sxs-lookup"><span data-stu-id="c6675-134">Id of the entity</span></span>|
|<span data-ttu-id="c6675-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="c6675-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="c6675-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6675-136">DateTimeOffset</span></span>|<span data-ttu-id="c6675-137">Carimbo de data/hora da última pulsação após o administrador integrado ao parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="c6675-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="c6675-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="c6675-138">partnerState</span></span>|[<span data-ttu-id="c6675-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="c6675-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="c6675-140">Estado do parceiro desse locatário.</span><span class="sxs-lookup"><span data-stu-id="c6675-140">Partner state of this tenant.</span></span> <span data-ttu-id="c6675-141">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="c6675-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="c6675-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c6675-142">displayName</span></span>|<span data-ttu-id="c6675-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6675-143">String</span></span>|<span data-ttu-id="c6675-144">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="c6675-144">Partner display name</span></span>|
|<span data-ttu-id="c6675-145">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="c6675-145">macOsOnboarded</span></span>|<span data-ttu-id="c6675-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="c6675-146">Boolean</span></span>|<span data-ttu-id="c6675-147">Parceiro integrado para dispositivos Mac.</span><span class="sxs-lookup"><span data-stu-id="c6675-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="c6675-148">windowsOnboarded</span><span class="sxs-lookup"><span data-stu-id="c6675-148">windowsOnboarded</span></span>|<span data-ttu-id="c6675-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="c6675-149">Boolean</span></span>|<span data-ttu-id="c6675-150">Parceiro integrado para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="c6675-150">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="c6675-151">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="c6675-151">androidOnboarded</span></span>|<span data-ttu-id="c6675-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="c6675-152">Boolean</span></span>|<span data-ttu-id="c6675-153">Parceiro integrado para dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="c6675-153">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="c6675-154">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="c6675-154">iosOnboarded</span></span>|<span data-ttu-id="c6675-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="c6675-155">Boolean</span></span>|<span data-ttu-id="c6675-156">Parceiro integrado para dispositivos IOS.</span><span class="sxs-lookup"><span data-stu-id="c6675-156">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="c6675-157">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c6675-157">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="c6675-158">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c6675-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c6675-159">Grupos de usuários que inscrevem dispositivos Mac por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c6675-159">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="c6675-160">windowsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c6675-160">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="c6675-161">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c6675-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c6675-162">Grupos de usuários que registram dispositivos do Windows por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c6675-162">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="c6675-163">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c6675-163">androidEnrollmentAssignments</span></span>|<span data-ttu-id="c6675-164">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c6675-164">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c6675-165">Grupos de usuários que registram dispositivos Android por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c6675-165">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="c6675-166">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c6675-166">iosEnrollmentAssignments</span></span>|<span data-ttu-id="c6675-167">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c6675-167">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c6675-168">Grupos de usuários que registram dispositivos IOS por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c6675-168">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="c6675-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6675-169">Response</span></span>
<span data-ttu-id="c6675-170">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6675-170">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6675-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6675-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6675-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6675-172">Request</span></span>
<span data-ttu-id="c6675-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6675-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
Content-type: application/json
Content-length: 1244

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c6675-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6675-174">Response</span></span>
<span data-ttu-id="c6675-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6675-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1293

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```






