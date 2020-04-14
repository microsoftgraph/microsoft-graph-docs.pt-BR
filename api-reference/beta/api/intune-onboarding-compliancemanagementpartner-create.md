---
title: Criar complianceManagementPartner
description: Criar um novo objeto complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c5a8ad9c45793b76b9c5a6432b5c349717086fcf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445490"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="c1160-103">Criar complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="c1160-103">Create complianceManagementPartner</span></span>

<span data-ttu-id="c1160-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1160-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1160-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c1160-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1160-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1160-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1160-107">Criar um novo objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="c1160-107">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1160-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c1160-108">Prerequisites</span></span>
<span data-ttu-id="c1160-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1160-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1160-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1160-111">Permission type</span></span>|<span data-ttu-id="c1160-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c1160-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1160-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1160-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1160-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1160-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c1160-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1160-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1160-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1160-116">Not supported.</span></span>|
|<span data-ttu-id="c1160-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1160-117">Application</span></span>|<span data-ttu-id="c1160-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1160-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1160-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1160-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="c1160-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1160-120">Request headers</span></span>
|<span data-ttu-id="c1160-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1160-121">Header</span></span>|<span data-ttu-id="c1160-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c1160-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1160-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1160-123">Authorization</span></span>|<span data-ttu-id="c1160-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1160-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1160-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c1160-125">Accept</span></span>|<span data-ttu-id="c1160-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1160-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1160-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1160-127">Request body</span></span>
<span data-ttu-id="c1160-128">No corpo da solicitação, forneça uma representação JSON do objeto complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="c1160-128">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="c1160-129">A tabela a seguir mostra as propriedades que são necessárias ao criar complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="c1160-129">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="c1160-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1160-130">Property</span></span>|<span data-ttu-id="c1160-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1160-131">Type</span></span>|<span data-ttu-id="c1160-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1160-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1160-133">id</span><span class="sxs-lookup"><span data-stu-id="c1160-133">id</span></span>|<span data-ttu-id="c1160-134">String</span><span class="sxs-lookup"><span data-stu-id="c1160-134">String</span></span>|<span data-ttu-id="c1160-135">ID da entidade</span><span class="sxs-lookup"><span data-stu-id="c1160-135">Id of the entity</span></span>|
|<span data-ttu-id="c1160-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="c1160-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="c1160-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1160-137">DateTimeOffset</span></span>|<span data-ttu-id="c1160-138">Carimbo de data/hora da última pulsação após o administrador integrado ao parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="c1160-138">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="c1160-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="c1160-139">partnerState</span></span>|[<span data-ttu-id="c1160-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="c1160-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="c1160-141">Estado do parceiro desse locatário.</span><span class="sxs-lookup"><span data-stu-id="c1160-141">Partner state of this tenant.</span></span> <span data-ttu-id="c1160-142">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="c1160-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="c1160-143">displayName</span><span class="sxs-lookup"><span data-stu-id="c1160-143">displayName</span></span>|<span data-ttu-id="c1160-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1160-144">String</span></span>|<span data-ttu-id="c1160-145">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="c1160-145">Partner display name</span></span>|
|<span data-ttu-id="c1160-146">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="c1160-146">macOsOnboarded</span></span>|<span data-ttu-id="c1160-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1160-147">Boolean</span></span>|<span data-ttu-id="c1160-148">Parceiro integrado para dispositivos Mac.</span><span class="sxs-lookup"><span data-stu-id="c1160-148">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="c1160-149">windowsOnboarded</span><span class="sxs-lookup"><span data-stu-id="c1160-149">windowsOnboarded</span></span>|<span data-ttu-id="c1160-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1160-150">Boolean</span></span>|<span data-ttu-id="c1160-151">Parceiro integrado para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="c1160-151">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="c1160-152">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="c1160-152">androidOnboarded</span></span>|<span data-ttu-id="c1160-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1160-153">Boolean</span></span>|<span data-ttu-id="c1160-154">Parceiro integrado para dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="c1160-154">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="c1160-155">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="c1160-155">iosOnboarded</span></span>|<span data-ttu-id="c1160-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1160-156">Boolean</span></span>|<span data-ttu-id="c1160-157">Parceiro integrado para dispositivos IOS.</span><span class="sxs-lookup"><span data-stu-id="c1160-157">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="c1160-158">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c1160-158">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="c1160-159">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c1160-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c1160-160">Grupos de usuários que inscrevem dispositivos Mac por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c1160-160">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="c1160-161">windowsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c1160-161">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="c1160-162">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c1160-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c1160-163">Grupos de usuários que registram dispositivos do Windows por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c1160-163">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="c1160-164">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c1160-164">androidEnrollmentAssignments</span></span>|<span data-ttu-id="c1160-165">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c1160-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c1160-166">Grupos de usuários que registram dispositivos Android por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c1160-166">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="c1160-167">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c1160-167">iosEnrollmentAssignments</span></span>|<span data-ttu-id="c1160-168">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c1160-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c1160-169">Grupos de usuários que registram dispositivos IOS por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c1160-169">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="c1160-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1160-170">Response</span></span>
<span data-ttu-id="c1160-171">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1160-171">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1160-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1160-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1160-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1160-173">Request</span></span>
<span data-ttu-id="c1160-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1160-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1160-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1160-175">Response</span></span>
<span data-ttu-id="c1160-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1160-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



