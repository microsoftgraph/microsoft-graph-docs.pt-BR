---
title: Atualizar windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary
description: Atualize as propriedades de um objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a32cbbc7ed88871838d75c5c917191179fe6ff3a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133889"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary"></a><span data-ttu-id="a6c57-103">Atualizar windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="a6c57-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span></span>

<span data-ttu-id="a6c57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6c57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6c57-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6c57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6c57-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6c57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6c57-107">Atualize as propriedades de um [objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)</span><span class="sxs-lookup"><span data-stu-id="a6c57-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6c57-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6c57-108">Prerequisites</span></span>
<span data-ttu-id="a6c57-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6c57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c57-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6c57-111">Permission type</span></span>|<span data-ttu-id="a6c57-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6c57-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6c57-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6c57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6c57-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c57-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a6c57-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6c57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6c57-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6c57-116">Not supported.</span></span>|
|<span data-ttu-id="a6c57-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6c57-117">Application</span></span>|<span data-ttu-id="a6c57-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c57-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6c57-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6c57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
```

## <a name="request-headers"></a><span data-ttu-id="a6c57-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c57-120">Request headers</span></span>
|<span data-ttu-id="a6c57-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6c57-121">Header</span></span>|<span data-ttu-id="a6c57-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a6c57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6c57-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6c57-123">Authorization</span></span>|<span data-ttu-id="a6c57-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6c57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6c57-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6c57-125">Accept</span></span>|<span data-ttu-id="a6c57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6c57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6c57-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c57-127">Request body</span></span>
<span data-ttu-id="a6c57-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)</span><span class="sxs-lookup"><span data-stu-id="a6c57-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="a6c57-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a6c57-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="a6c57-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6c57-130">Property</span></span>|<span data-ttu-id="a6c57-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6c57-131">Type</span></span>|<span data-ttu-id="a6c57-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6c57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6c57-133">id</span><span class="sxs-lookup"><span data-stu-id="a6c57-133">id</span></span>|<span data-ttu-id="a6c57-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6c57-134">String</span></span>|<span data-ttu-id="a6c57-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a6c57-135">Key of the entity.</span></span>|
|<span data-ttu-id="a6c57-136">deployedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6c57-136">deployedDeviceCount</span></span>|<span data-ttu-id="a6c57-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a6c57-137">Int32</span></span>|<span data-ttu-id="a6c57-138">Número de dispositivos que implantaram com êxito esta política suplementar WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="a6c57-138">Number of Devices that have successfully deployed this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="a6c57-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6c57-139">failedDeviceCount</span></span>|<span data-ttu-id="a6c57-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a6c57-140">Int32</span></span>|<span data-ttu-id="a6c57-141">Número de dispositivos que falharam na implantação dessa política complementar windowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="a6c57-141">Number of Devices that have failed to deploy this WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="a6c57-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6c57-142">Response</span></span>
<span data-ttu-id="a6c57-143">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6c57-143">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6c57-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6c57-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6c57-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c57-145">Request</span></span>
<span data-ttu-id="a6c57-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6c57-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a6c57-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6c57-147">Response</span></span>
<span data-ttu-id="a6c57-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6c57-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




