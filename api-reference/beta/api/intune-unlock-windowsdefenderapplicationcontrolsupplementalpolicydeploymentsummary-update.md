---
title: Atualizar windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary
description: Atualiza as propriedades de um objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e04b7598cad9e8e577575b581e0370fc99930f15
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454357"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary"></a><span data-ttu-id="2833f-103">Atualizar windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="2833f-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span></span>

<span data-ttu-id="2833f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2833f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2833f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2833f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2833f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2833f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2833f-107">Atualiza as propriedades de um objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="2833f-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2833f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2833f-108">Prerequisites</span></span>
<span data-ttu-id="2833f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2833f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2833f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2833f-111">Permission type</span></span>|<span data-ttu-id="2833f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2833f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2833f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2833f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2833f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2833f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2833f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2833f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2833f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2833f-116">Not supported.</span></span>|
|<span data-ttu-id="2833f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2833f-117">Application</span></span>|<span data-ttu-id="2833f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2833f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2833f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2833f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
```

## <a name="request-headers"></a><span data-ttu-id="2833f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2833f-120">Request headers</span></span>
|<span data-ttu-id="2833f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2833f-121">Header</span></span>|<span data-ttu-id="2833f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2833f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2833f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2833f-123">Authorization</span></span>|<span data-ttu-id="2833f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2833f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2833f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2833f-125">Accept</span></span>|<span data-ttu-id="2833f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2833f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2833f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2833f-127">Request body</span></span>
<span data-ttu-id="2833f-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="2833f-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="2833f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2833f-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="2833f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2833f-130">Property</span></span>|<span data-ttu-id="2833f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2833f-131">Type</span></span>|<span data-ttu-id="2833f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2833f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2833f-133">id</span><span class="sxs-lookup"><span data-stu-id="2833f-133">id</span></span>|<span data-ttu-id="2833f-134">String</span><span class="sxs-lookup"><span data-stu-id="2833f-134">String</span></span>|<span data-ttu-id="2833f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2833f-135">Key of the entity.</span></span>|
|<span data-ttu-id="2833f-136">deployedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2833f-136">deployedDeviceCount</span></span>|<span data-ttu-id="2833f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2833f-137">Int32</span></span>|<span data-ttu-id="2833f-138">Número de dispositivos que implantaram com êxito esta política suplementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="2833f-138">Number of Devices that have successfully deployed this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="2833f-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2833f-139">failedDeviceCount</span></span>|<span data-ttu-id="2833f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2833f-140">Int32</span></span>|<span data-ttu-id="2833f-141">Número de dispositivos que falharam ao implantar esta política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="2833f-141">Number of Devices that have failed to deploy this WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="2833f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2833f-142">Response</span></span>
<span data-ttu-id="2833f-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2833f-143">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2833f-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2833f-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="2833f-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2833f-145">Request</span></span>
<span data-ttu-id="2833f-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2833f-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
  "deployedDeviceCount": 3,
  "failedDeviceCount": 1
}
```

### <a name="response"></a><span data-ttu-id="2833f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2833f-147">Response</span></span>
<span data-ttu-id="2833f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2833f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
  "id": "2f8656ed-56ed-2f86-ed56-862fed56862f",
  "deployedDeviceCount": 3,
  "failedDeviceCount": 1
}
```



