---
title: Criar complianceManagementPartner
description: Crie um novo objeto complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0779afeef4d9b3944c5bd4c40b9222bf59b4fe09
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758042"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="5b907-103">Criar complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="5b907-103">Create complianceManagementPartner</span></span>

<span data-ttu-id="5b907-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b907-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b907-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b907-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b907-106">Crie um novo [objeto complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="5b907-106">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b907-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b907-107">Prerequisites</span></span>
<span data-ttu-id="5b907-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b907-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b907-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b907-110">Permission type</span></span>|<span data-ttu-id="5b907-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b907-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b907-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b907-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b907-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b907-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5b907-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b907-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b907-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b907-115">Not supported.</span></span>|
|<span data-ttu-id="5b907-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b907-116">Application</span></span>|<span data-ttu-id="5b907-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b907-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b907-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b907-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="5b907-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b907-119">Request headers</span></span>
|<span data-ttu-id="5b907-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b907-120">Header</span></span>|<span data-ttu-id="5b907-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5b907-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b907-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b907-122">Authorization</span></span>|<span data-ttu-id="5b907-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b907-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b907-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b907-124">Accept</span></span>|<span data-ttu-id="5b907-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b907-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b907-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b907-126">Request body</span></span>
<span data-ttu-id="5b907-127">No corpo da solicitação, fornece uma representação JSON para o objeto complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="5b907-127">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="5b907-128">A tabela a seguir mostra as propriedades que são necessárias ao criar complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="5b907-128">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="5b907-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b907-129">Property</span></span>|<span data-ttu-id="5b907-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b907-130">Type</span></span>|<span data-ttu-id="5b907-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b907-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b907-132">id</span><span class="sxs-lookup"><span data-stu-id="5b907-132">id</span></span>|<span data-ttu-id="5b907-133">String</span><span class="sxs-lookup"><span data-stu-id="5b907-133">String</span></span>|<span data-ttu-id="5b907-134">ID da entidade</span><span class="sxs-lookup"><span data-stu-id="5b907-134">Id of the entity</span></span>|
|<span data-ttu-id="5b907-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="5b907-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="5b907-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b907-136">DateTimeOffset</span></span>|<span data-ttu-id="5b907-137">Timestamp de última pulsação depois que o administrador entrou no parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="5b907-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="5b907-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="5b907-138">partnerState</span></span>|[<span data-ttu-id="5b907-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="5b907-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="5b907-140">Estado do parceiro desse locatário.</span><span class="sxs-lookup"><span data-stu-id="5b907-140">Partner state of this tenant.</span></span> <span data-ttu-id="5b907-141">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="5b907-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="5b907-142">displayName</span><span class="sxs-lookup"><span data-stu-id="5b907-142">displayName</span></span>|<span data-ttu-id="5b907-143">String</span><span class="sxs-lookup"><span data-stu-id="5b907-143">String</span></span>|<span data-ttu-id="5b907-144">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="5b907-144">Partner display name</span></span>|
|<span data-ttu-id="5b907-145">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="5b907-145">macOsOnboarded</span></span>|<span data-ttu-id="5b907-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="5b907-146">Boolean</span></span>|<span data-ttu-id="5b907-147">Parceiro a bordo para dispositivos Mac.</span><span class="sxs-lookup"><span data-stu-id="5b907-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="5b907-148">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="5b907-148">androidOnboarded</span></span>|<span data-ttu-id="5b907-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="5b907-149">Boolean</span></span>|<span data-ttu-id="5b907-150">Parceiro a bordo para dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="5b907-150">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="5b907-151">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="5b907-151">iosOnboarded</span></span>|<span data-ttu-id="5b907-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="5b907-152">Boolean</span></span>|<span data-ttu-id="5b907-153">Parceiro internado para dispositivos ios.</span><span class="sxs-lookup"><span data-stu-id="5b907-153">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="5b907-154">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="5b907-154">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="5b907-155">[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5b907-155">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="5b907-156">Grupos de usuários que registram dispositivos Mac por meio de parceiros.</span><span class="sxs-lookup"><span data-stu-id="5b907-156">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="5b907-157">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="5b907-157">androidEnrollmentAssignments</span></span>|<span data-ttu-id="5b907-158">[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5b907-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="5b907-159">Grupos de usuários que registram dispositivos Android por meio de parceiros.</span><span class="sxs-lookup"><span data-stu-id="5b907-159">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="5b907-160">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="5b907-160">iosEnrollmentAssignments</span></span>|<span data-ttu-id="5b907-161">[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5b907-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="5b907-162">Grupos de usuários que registram dispositivos ios por meio de parceiros.</span><span class="sxs-lookup"><span data-stu-id="5b907-162">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="5b907-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b907-163">Response</span></span>
<span data-ttu-id="5b907-164">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b907-164">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b907-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b907-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b907-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b907-166">Request</span></span>
<span data-ttu-id="5b907-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b907-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners
Content-type: application/json
Content-length: 1186

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5b907-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b907-168">Response</span></span>
<span data-ttu-id="5b907-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b907-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1235

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




