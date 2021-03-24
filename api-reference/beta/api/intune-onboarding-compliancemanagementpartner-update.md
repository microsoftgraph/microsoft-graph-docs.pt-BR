---
title: Atualizar complianceManagementPartner
description: Atualize as propriedades de um objeto complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c8cfa6c03236e7c75713eeb4c7c915a21fbef789
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135149"
---
# <a name="update-compliancemanagementpartner"></a><span data-ttu-id="a0e85-103">Atualizar complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a0e85-103">Update complianceManagementPartner</span></span>

<span data-ttu-id="a0e85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0e85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0e85-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0e85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0e85-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0e85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0e85-107">Atualize as propriedades de [um objeto complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="a0e85-107">Update the properties of a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0e85-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0e85-108">Prerequisites</span></span>
<span data-ttu-id="a0e85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0e85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0e85-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0e85-111">Permission type</span></span>|<span data-ttu-id="a0e85-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0e85-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0e85-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0e85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0e85-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0e85-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a0e85-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0e85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0e85-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0e85-116">Not supported.</span></span>|
|<span data-ttu-id="a0e85-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0e85-117">Application</span></span>|<span data-ttu-id="a0e85-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0e85-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0e85-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0e85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="a0e85-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0e85-120">Request headers</span></span>
|<span data-ttu-id="a0e85-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0e85-121">Header</span></span>|<span data-ttu-id="a0e85-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0e85-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0e85-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0e85-123">Authorization</span></span>|<span data-ttu-id="a0e85-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0e85-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0e85-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0e85-125">Accept</span></span>|<span data-ttu-id="a0e85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0e85-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0e85-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0e85-127">Request body</span></span>
<span data-ttu-id="a0e85-128">No corpo da solicitação, fornece uma representação JSON para o [objeto complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="a0e85-128">In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

<span data-ttu-id="a0e85-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="a0e85-129">The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

|<span data-ttu-id="a0e85-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0e85-130">Property</span></span>|<span data-ttu-id="a0e85-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0e85-131">Type</span></span>|<span data-ttu-id="a0e85-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0e85-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0e85-133">id</span><span class="sxs-lookup"><span data-stu-id="a0e85-133">id</span></span>|<span data-ttu-id="a0e85-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0e85-134">String</span></span>|<span data-ttu-id="a0e85-135">ID da entidade</span><span class="sxs-lookup"><span data-stu-id="a0e85-135">Id of the entity</span></span>|
|<span data-ttu-id="a0e85-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="a0e85-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="a0e85-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0e85-137">DateTimeOffset</span></span>|<span data-ttu-id="a0e85-138">Timestamp de última pulsação depois que o administrador entrou no parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="a0e85-138">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="a0e85-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="a0e85-139">partnerState</span></span>|[<span data-ttu-id="a0e85-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="a0e85-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="a0e85-141">Estado do parceiro desse locatário.</span><span class="sxs-lookup"><span data-stu-id="a0e85-141">Partner state of this tenant.</span></span> <span data-ttu-id="a0e85-142">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="a0e85-143">displayName</span><span class="sxs-lookup"><span data-stu-id="a0e85-143">displayName</span></span>|<span data-ttu-id="a0e85-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0e85-144">String</span></span>|<span data-ttu-id="a0e85-145">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="a0e85-145">Partner display name</span></span>|
|<span data-ttu-id="a0e85-146">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="a0e85-146">macOsOnboarded</span></span>|<span data-ttu-id="a0e85-147">Booleano</span><span class="sxs-lookup"><span data-stu-id="a0e85-147">Boolean</span></span>|<span data-ttu-id="a0e85-148">Parceiro a bordo para dispositivos Mac.</span><span class="sxs-lookup"><span data-stu-id="a0e85-148">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="a0e85-149">windowsOnboarded</span><span class="sxs-lookup"><span data-stu-id="a0e85-149">windowsOnboarded</span></span>|<span data-ttu-id="a0e85-150">Booleano</span><span class="sxs-lookup"><span data-stu-id="a0e85-150">Boolean</span></span>|<span data-ttu-id="a0e85-151">Parceiro a bordo para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="a0e85-151">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="a0e85-152">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="a0e85-152">androidOnboarded</span></span>|<span data-ttu-id="a0e85-153">Booleano</span><span class="sxs-lookup"><span data-stu-id="a0e85-153">Boolean</span></span>|<span data-ttu-id="a0e85-154">Parceiro a bordo para dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="a0e85-154">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="a0e85-155">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="a0e85-155">iosOnboarded</span></span>|<span data-ttu-id="a0e85-156">Booleano</span><span class="sxs-lookup"><span data-stu-id="a0e85-156">Boolean</span></span>|<span data-ttu-id="a0e85-157">Parceiro internado para dispositivos ios.</span><span class="sxs-lookup"><span data-stu-id="a0e85-157">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="a0e85-158">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="a0e85-158">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="a0e85-159">[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a0e85-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="a0e85-160">Grupos de usuários que registram dispositivos Mac por meio de parceiros.</span><span class="sxs-lookup"><span data-stu-id="a0e85-160">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="a0e85-161">windowsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="a0e85-161">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="a0e85-162">[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a0e85-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="a0e85-163">Grupos de usuários que registram dispositivos Windows por meio de parceiros.</span><span class="sxs-lookup"><span data-stu-id="a0e85-163">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="a0e85-164">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="a0e85-164">androidEnrollmentAssignments</span></span>|<span data-ttu-id="a0e85-165">[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a0e85-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="a0e85-166">Grupos de usuários que registram dispositivos Android por meio de parceiros.</span><span class="sxs-lookup"><span data-stu-id="a0e85-166">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="a0e85-167">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="a0e85-167">iosEnrollmentAssignments</span></span>|<span data-ttu-id="a0e85-168">[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a0e85-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="a0e85-169">Grupos de usuários que registram dispositivos ios por meio de parceiros.</span><span class="sxs-lookup"><span data-stu-id="a0e85-169">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="a0e85-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0e85-170">Response</span></span>
<span data-ttu-id="a0e85-171">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0e85-171">If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0e85-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0e85-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0e85-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0e85-173">Request</span></span>
<span data-ttu-id="a0e85-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0e85-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
Content-type: application/json
Content-length: 2216

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a0e85-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0e85-175">Response</span></span>
<span data-ttu-id="a0e85-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0e85-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2265

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




