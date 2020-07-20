---
title: Criar complianceManagementPartner
description: Criar um novo objeto complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c606f0fdf4fbf9f589c2aab2423373225f1bdf7c
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744108"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="345ff-103">Criar complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="345ff-103">Create complianceManagementPartner</span></span>

<span data-ttu-id="345ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="345ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="345ff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="345ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="345ff-106">Criar um novo objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="345ff-106">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="345ff-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="345ff-107">Prerequisites</span></span>
<span data-ttu-id="345ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="345ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="345ff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="345ff-110">Permission type</span></span>|<span data-ttu-id="345ff-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="345ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="345ff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="345ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="345ff-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="345ff-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="345ff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="345ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="345ff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="345ff-115">Not supported.</span></span>|
|<span data-ttu-id="345ff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="345ff-116">Application</span></span>|<span data-ttu-id="345ff-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="345ff-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="345ff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="345ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="345ff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="345ff-119">Request headers</span></span>
|<span data-ttu-id="345ff-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="345ff-120">Header</span></span>|<span data-ttu-id="345ff-121">Valor</span><span class="sxs-lookup"><span data-stu-id="345ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="345ff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="345ff-122">Authorization</span></span>|<span data-ttu-id="345ff-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="345ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="345ff-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="345ff-124">Accept</span></span>|<span data-ttu-id="345ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="345ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="345ff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="345ff-126">Request body</span></span>
<span data-ttu-id="345ff-127">No corpo da solicitação, forneça uma representação JSON do objeto complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="345ff-127">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="345ff-128">A tabela a seguir mostra as propriedades que são necessárias ao criar complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="345ff-128">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="345ff-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="345ff-129">Property</span></span>|<span data-ttu-id="345ff-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="345ff-130">Type</span></span>|<span data-ttu-id="345ff-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="345ff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="345ff-132">id</span><span class="sxs-lookup"><span data-stu-id="345ff-132">id</span></span>|<span data-ttu-id="345ff-133">String</span><span class="sxs-lookup"><span data-stu-id="345ff-133">String</span></span>|<span data-ttu-id="345ff-134">ID da entidade</span><span class="sxs-lookup"><span data-stu-id="345ff-134">Id of the entity</span></span>|
|<span data-ttu-id="345ff-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="345ff-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="345ff-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="345ff-136">DateTimeOffset</span></span>|<span data-ttu-id="345ff-137">Carimbo de data/hora da última pulsação após o administrador integrado ao parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="345ff-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="345ff-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="345ff-138">partnerState</span></span>|[<span data-ttu-id="345ff-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="345ff-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="345ff-140">Estado do parceiro desse locatário.</span><span class="sxs-lookup"><span data-stu-id="345ff-140">Partner state of this tenant.</span></span> <span data-ttu-id="345ff-141">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="345ff-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="345ff-142">displayName</span><span class="sxs-lookup"><span data-stu-id="345ff-142">displayName</span></span>|<span data-ttu-id="345ff-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="345ff-143">String</span></span>|<span data-ttu-id="345ff-144">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="345ff-144">Partner display name</span></span>|
|<span data-ttu-id="345ff-145">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="345ff-145">macOsOnboarded</span></span>|<span data-ttu-id="345ff-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="345ff-146">Boolean</span></span>|<span data-ttu-id="345ff-147">Parceiro integrado para dispositivos Mac.</span><span class="sxs-lookup"><span data-stu-id="345ff-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="345ff-148">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="345ff-148">androidOnboarded</span></span>|<span data-ttu-id="345ff-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="345ff-149">Boolean</span></span>|<span data-ttu-id="345ff-150">Parceiro integrado para dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="345ff-150">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="345ff-151">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="345ff-151">iosOnboarded</span></span>|<span data-ttu-id="345ff-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="345ff-152">Boolean</span></span>|<span data-ttu-id="345ff-153">Parceiro integrado para dispositivos IOS.</span><span class="sxs-lookup"><span data-stu-id="345ff-153">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="345ff-154">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="345ff-154">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="345ff-155">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="345ff-155">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="345ff-156">Grupos de usuários que inscrevem dispositivos Mac por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="345ff-156">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="345ff-157">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="345ff-157">androidEnrollmentAssignments</span></span>|<span data-ttu-id="345ff-158">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="345ff-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="345ff-159">Grupos de usuários que registram dispositivos Android por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="345ff-159">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="345ff-160">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="345ff-160">iosEnrollmentAssignments</span></span>|<span data-ttu-id="345ff-161">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="345ff-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="345ff-162">Grupos de usuários que registram dispositivos IOS por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="345ff-162">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="345ff-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="345ff-163">Response</span></span>
<span data-ttu-id="345ff-164">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="345ff-164">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="345ff-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="345ff-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="345ff-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="345ff-166">Request</span></span>
<span data-ttu-id="345ff-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="345ff-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners
Content-type: application/json
Content-length: 982

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
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

### <a name="response"></a><span data-ttu-id="345ff-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="345ff-168">Response</span></span>
<span data-ttu-id="345ff-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="345ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1031

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
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



