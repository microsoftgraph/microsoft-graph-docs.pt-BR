---
title: Atualizar windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary
description: Atualiza as propriedades de um objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95b43a19625b4501d385c683cb463f32ed42def0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938520"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary"></a><span data-ttu-id="1f416-103">Atualizar windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="1f416-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span></span>

> <span data-ttu-id="1f416-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1f416-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f416-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f416-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f416-106">Atualiza as propriedades de um objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="1f416-106">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f416-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1f416-107">Prerequisites</span></span>
<span data-ttu-id="1f416-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f416-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f416-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f416-110">Permission type</span></span>|<span data-ttu-id="1f416-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1f416-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f416-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f416-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f416-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f416-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1f416-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f416-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f416-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f416-115">Not supported.</span></span>|
|<span data-ttu-id="1f416-116">Application</span><span class="sxs-lookup"><span data-stu-id="1f416-116">Application</span></span>|<span data-ttu-id="1f416-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f416-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f416-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f416-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
```

## <a name="request-headers"></a><span data-ttu-id="1f416-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f416-119">Request headers</span></span>
|<span data-ttu-id="1f416-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f416-120">Header</span></span>|<span data-ttu-id="1f416-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1f416-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f416-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f416-122">Authorization</span></span>|<span data-ttu-id="1f416-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f416-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f416-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1f416-124">Accept</span></span>|<span data-ttu-id="1f416-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f416-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f416-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f416-126">Request body</span></span>
<span data-ttu-id="1f416-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="1f416-127">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="1f416-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="1f416-128">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="1f416-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f416-129">Property</span></span>|<span data-ttu-id="1f416-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f416-130">Type</span></span>|<span data-ttu-id="1f416-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f416-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f416-132">id</span><span class="sxs-lookup"><span data-stu-id="1f416-132">id</span></span>|<span data-ttu-id="1f416-133">String</span><span class="sxs-lookup"><span data-stu-id="1f416-133">String</span></span>|<span data-ttu-id="1f416-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1f416-134">Key of the entity.</span></span>|
|<span data-ttu-id="1f416-135">deployedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1f416-135">deployedDeviceCount</span></span>|<span data-ttu-id="1f416-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1f416-136">Int32</span></span>|<span data-ttu-id="1f416-137">Número de dispositivos que implantaram com êxito esta política suplementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="1f416-137">Number of Devices that have successfully deployed this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="1f416-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1f416-138">failedDeviceCount</span></span>|<span data-ttu-id="1f416-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1f416-139">Int32</span></span>|<span data-ttu-id="1f416-140">Número de dispositivos que falharam ao implantar esta política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="1f416-140">Number of Devices that have failed to deploy this WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="1f416-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f416-141">Response</span></span>
<span data-ttu-id="1f416-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f416-142">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f416-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f416-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f416-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f416-144">Request</span></span>
<span data-ttu-id="1f416-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f416-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f416-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f416-146">Response</span></span>
<span data-ttu-id="1f416-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f416-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





