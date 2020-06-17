---
title: Atualizar complianceManagementPartner
description: Atualiza as propriedades de um objeto complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9574c2ddaacb60f9c41ea73608445de93365cb6e
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744105"
---
# <a name="update-compliancemanagementpartner"></a><span data-ttu-id="ec5ac-103">Atualizar complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="ec5ac-103">Update complianceManagementPartner</span></span>

<span data-ttu-id="ec5ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec5ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec5ac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec5ac-106">Atualiza as propriedades de um objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="ec5ac-106">Update the properties of a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec5ac-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec5ac-107">Prerequisites</span></span>
<span data-ttu-id="ec5ac-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ec5ac-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec5ac-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec5ac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec5ac-110">Permission type</span></span>|<span data-ttu-id="ec5ac-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ec5ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec5ac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec5ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec5ac-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec5ac-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ec5ac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec5ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec5ac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-115">Not supported.</span></span>|
|<span data-ttu-id="ec5ac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec5ac-116">Application</span></span>|<span data-ttu-id="ec5ac-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec5ac-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec5ac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec5ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="ec5ac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec5ac-119">Request headers</span></span>
|<span data-ttu-id="ec5ac-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec5ac-120">Header</span></span>|<span data-ttu-id="ec5ac-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ec5ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec5ac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec5ac-122">Authorization</span></span>|<span data-ttu-id="ec5ac-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec5ac-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec5ac-124">Accept</span></span>|<span data-ttu-id="ec5ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ec5ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec5ac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec5ac-126">Request body</span></span>
<span data-ttu-id="ec5ac-127">No corpo da solicitação, forneça uma representação JSON do objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="ec5ac-127">In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

<span data-ttu-id="ec5ac-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="ec5ac-128">The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

|<span data-ttu-id="ec5ac-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec5ac-129">Property</span></span>|<span data-ttu-id="ec5ac-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec5ac-130">Type</span></span>|<span data-ttu-id="ec5ac-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec5ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec5ac-132">id</span><span class="sxs-lookup"><span data-stu-id="ec5ac-132">id</span></span>|<span data-ttu-id="ec5ac-133">String</span><span class="sxs-lookup"><span data-stu-id="ec5ac-133">String</span></span>|<span data-ttu-id="ec5ac-134">ID da entidade</span><span class="sxs-lookup"><span data-stu-id="ec5ac-134">Id of the entity</span></span>|
|<span data-ttu-id="ec5ac-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="ec5ac-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="ec5ac-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec5ac-136">DateTimeOffset</span></span>|<span data-ttu-id="ec5ac-137">Carimbo de data/hora da última pulsação após o administrador integrado ao parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="ec5ac-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="ec5ac-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="ec5ac-138">partnerState</span></span>|[<span data-ttu-id="ec5ac-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="ec5ac-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="ec5ac-140">Estado do parceiro desse locatário.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-140">Partner state of this tenant.</span></span> <span data-ttu-id="ec5ac-141">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="ec5ac-142">displayName</span><span class="sxs-lookup"><span data-stu-id="ec5ac-142">displayName</span></span>|<span data-ttu-id="ec5ac-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec5ac-143">String</span></span>|<span data-ttu-id="ec5ac-144">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="ec5ac-144">Partner display name</span></span>|
|<span data-ttu-id="ec5ac-145">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="ec5ac-145">macOsOnboarded</span></span>|<span data-ttu-id="ec5ac-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec5ac-146">Boolean</span></span>|<span data-ttu-id="ec5ac-147">Parceiro integrado para dispositivos Mac.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="ec5ac-148">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="ec5ac-148">androidOnboarded</span></span>|<span data-ttu-id="ec5ac-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec5ac-149">Boolean</span></span>|<span data-ttu-id="ec5ac-150">Parceiro integrado para dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-150">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="ec5ac-151">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="ec5ac-151">iosOnboarded</span></span>|<span data-ttu-id="ec5ac-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec5ac-152">Boolean</span></span>|<span data-ttu-id="ec5ac-153">Parceiro integrado para dispositivos IOS.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-153">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="ec5ac-154">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="ec5ac-154">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="ec5ac-155">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ec5ac-155">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="ec5ac-156">Grupos de usuários que inscrevem dispositivos Mac por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-156">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="ec5ac-157">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="ec5ac-157">androidEnrollmentAssignments</span></span>|<span data-ttu-id="ec5ac-158">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ec5ac-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="ec5ac-159">Grupos de usuários que registram dispositivos Android por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-159">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="ec5ac-160">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="ec5ac-160">iosEnrollmentAssignments</span></span>|<span data-ttu-id="ec5ac-161">coleção [complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ec5ac-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="ec5ac-162">Grupos de usuários que registram dispositivos IOS por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-162">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="ec5ac-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec5ac-163">Response</span></span>
<span data-ttu-id="ec5ac-164">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-164">If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec5ac-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec5ac-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec5ac-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec5ac-166">Request</span></span>
<span data-ttu-id="ec5ac-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
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

### <a name="response"></a><span data-ttu-id="ec5ac-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec5ac-168">Response</span></span>
<span data-ttu-id="ec5ac-169">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-169">Here is an example of the response.</span></span> <span data-ttu-id="ec5ac-170">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-170">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ec5ac-171">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ec5ac-171">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



