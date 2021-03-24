---
title: Criar userExperienceAnalyticsRemoteConnection
description: Crie um novo objeto userExperienceAnalyticsRemoteConnection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d044809eebf198e4347bb6182388cb7096fa882d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135968"
---
# <a name="create-userexperienceanalyticsremoteconnection"></a><span data-ttu-id="81b8f-103">Criar userExperienceAnalyticsRemoteConnection</span><span class="sxs-lookup"><span data-stu-id="81b8f-103">Create userExperienceAnalyticsRemoteConnection</span></span>

<span data-ttu-id="81b8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81b8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81b8f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81b8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81b8f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81b8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81b8f-107">Crie um novo [objeto userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)</span><span class="sxs-lookup"><span data-stu-id="81b8f-107">Create a new [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81b8f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81b8f-108">Prerequisites</span></span>
<span data-ttu-id="81b8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81b8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81b8f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81b8f-111">Permission type</span></span>|<span data-ttu-id="81b8f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81b8f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81b8f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81b8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81b8f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81b8f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="81b8f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81b8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81b8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81b8f-116">Not supported.</span></span>|
|<span data-ttu-id="81b8f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81b8f-117">Application</span></span>|<span data-ttu-id="81b8f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81b8f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81b8f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81b8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsRemoteConnection
```

## <a name="request-headers"></a><span data-ttu-id="81b8f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81b8f-120">Request headers</span></span>
|<span data-ttu-id="81b8f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81b8f-121">Header</span></span>|<span data-ttu-id="81b8f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="81b8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81b8f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="81b8f-123">Authorization</span></span>|<span data-ttu-id="81b8f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81b8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81b8f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81b8f-125">Accept</span></span>|<span data-ttu-id="81b8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81b8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81b8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81b8f-127">Request body</span></span>
<span data-ttu-id="81b8f-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsRemoteConnection.</span><span class="sxs-lookup"><span data-stu-id="81b8f-128">In the request body, supply a JSON representation for the userExperienceAnalyticsRemoteConnection object.</span></span>

<span data-ttu-id="81b8f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsRemoteConnection.</span><span class="sxs-lookup"><span data-stu-id="81b8f-129">The following table shows the properties that are required when you create the userExperienceAnalyticsRemoteConnection.</span></span>

|<span data-ttu-id="81b8f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81b8f-130">Property</span></span>|<span data-ttu-id="81b8f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="81b8f-131">Type</span></span>|<span data-ttu-id="81b8f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="81b8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81b8f-133">id</span><span class="sxs-lookup"><span data-stu-id="81b8f-133">id</span></span>|<span data-ttu-id="81b8f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81b8f-134">String</span></span>|<span data-ttu-id="81b8f-135">O identificador exclusivo da entidade de conexão remota de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="81b8f-135">The unique identifier of the user experience analytics remote connection entity.</span></span>|
|<span data-ttu-id="81b8f-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="81b8f-136">deviceId</span></span>|<span data-ttu-id="81b8f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81b8f-137">String</span></span>|<span data-ttu-id="81b8f-138">A id do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81b8f-138">The id of the device.</span></span>|
|<span data-ttu-id="81b8f-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="81b8f-139">deviceName</span></span>|<span data-ttu-id="81b8f-140">String</span><span class="sxs-lookup"><span data-stu-id="81b8f-140">String</span></span>|<span data-ttu-id="81b8f-141">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81b8f-141">The name of the device.</span></span>|
|<span data-ttu-id="81b8f-142">modelo</span><span class="sxs-lookup"><span data-stu-id="81b8f-142">model</span></span>|<span data-ttu-id="81b8f-143">String</span><span class="sxs-lookup"><span data-stu-id="81b8f-143">String</span></span>|<span data-ttu-id="81b8f-144">O modelo de dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="81b8f-144">The user experience analytics device model.</span></span>|
|<span data-ttu-id="81b8f-145">virtualNetwork</span><span class="sxs-lookup"><span data-stu-id="81b8f-145">virtualNetwork</span></span>|<span data-ttu-id="81b8f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81b8f-146">String</span></span>|<span data-ttu-id="81b8f-147">A rede virtual de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="81b8f-147">The user experience analytics virtual network.</span></span>|
|<span data-ttu-id="81b8f-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="81b8f-148">deviceCount</span></span>|<span data-ttu-id="81b8f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="81b8f-149">Int32</span></span>|<span data-ttu-id="81b8f-150">A contagem de conexão remota.</span><span class="sxs-lookup"><span data-stu-id="81b8f-150">The count of remote connection.</span></span> <span data-ttu-id="81b8f-151">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="81b8f-151">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="81b8f-152">cloudPcRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="81b8f-152">cloudPcRoundTripTime</span></span>|<span data-ttu-id="81b8f-153">Duplo</span><span class="sxs-lookup"><span data-stu-id="81b8f-153">Double</span></span>|<span data-ttu-id="81b8f-154">O tempo de dica de ida e volta do dispositivo cloud pc.</span><span class="sxs-lookup"><span data-stu-id="81b8f-154">The round tip time of Cloud PC Device.</span></span> <span data-ttu-id="81b8f-155">Valores válidos de 0 a 1,79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="81b8f-155">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="81b8f-156">cloudPcSignInTime</span><span class="sxs-lookup"><span data-stu-id="81b8f-156">cloudPcSignInTime</span></span>|<span data-ttu-id="81b8f-157">Duplo</span><span class="sxs-lookup"><span data-stu-id="81b8f-157">Double</span></span>|<span data-ttu-id="81b8f-158">A hora de entrada do dispositivo cloud pc.</span><span class="sxs-lookup"><span data-stu-id="81b8f-158">The sign in time of Cloud PC Device.</span></span> <span data-ttu-id="81b8f-159">Valores válidos de 0 a 1,79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="81b8f-159">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="81b8f-160">remoteSignInTime</span><span class="sxs-lookup"><span data-stu-id="81b8f-160">remoteSignInTime</span></span>|<span data-ttu-id="81b8f-161">Duplo</span><span class="sxs-lookup"><span data-stu-id="81b8f-161">Double</span></span>|<span data-ttu-id="81b8f-162">A hora de entrada remota do dispositivo cloud pc.</span><span class="sxs-lookup"><span data-stu-id="81b8f-162">The remote sign in time of Cloud PC Device.</span></span> <span data-ttu-id="81b8f-163">Valores válidos de 0 a 1,79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="81b8f-163">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="81b8f-164">coreBootTime</span><span class="sxs-lookup"><span data-stu-id="81b8f-164">coreBootTime</span></span>|<span data-ttu-id="81b8f-165">Duplo</span><span class="sxs-lookup"><span data-stu-id="81b8f-165">Double</span></span>|<span data-ttu-id="81b8f-166">O tempo de inicialização principal do Dispositivo cloud pc.</span><span class="sxs-lookup"><span data-stu-id="81b8f-166">The core boot time of Cloud PC Device.</span></span> <span data-ttu-id="81b8f-167">Valores válidos de 0 a 1,79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="81b8f-167">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="81b8f-168">coreSignInTime</span><span class="sxs-lookup"><span data-stu-id="81b8f-168">coreSignInTime</span></span>|<span data-ttu-id="81b8f-169">Duplo</span><span class="sxs-lookup"><span data-stu-id="81b8f-169">Double</span></span>|<span data-ttu-id="81b8f-170">A hora de entrada principal do dispositivo cloud pc.</span><span class="sxs-lookup"><span data-stu-id="81b8f-170">The core sign in time of Cloud PC Device.</span></span> <span data-ttu-id="81b8f-171">Valores válidos de 0 a 1,79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="81b8f-171">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="81b8f-172">cloudPcFailurePercentage</span><span class="sxs-lookup"><span data-stu-id="81b8f-172">cloudPcFailurePercentage</span></span>|<span data-ttu-id="81b8f-173">Duplo</span><span class="sxs-lookup"><span data-stu-id="81b8f-173">Double</span></span>|<span data-ttu-id="81b8f-174">A porcentagem de falha de entrada do dispositivo cloud pc.</span><span class="sxs-lookup"><span data-stu-id="81b8f-174">The sign in failure percentage of Cloud PC Device.</span></span> <span data-ttu-id="81b8f-175">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="81b8f-175">Valid values 0 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="81b8f-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b8f-176">Response</span></span>
<span data-ttu-id="81b8f-177">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81b8f-177">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81b8f-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81b8f-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="81b8f-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81b8f-179">Request</span></span>
<span data-ttu-id="81b8f-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81b8f-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection
Content-type: application/json
Content-length: 479

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "virtualNetwork": "Virtual Network value",
  "deviceCount": 11,
  "cloudPcRoundTripTime": 6.666666666666667,
  "cloudPcSignInTime": 5.666666666666667,
  "remoteSignInTime": 5.333333333333333,
  "coreBootTime": 4.0,
  "coreSignInTime": 4.666666666666667,
  "cloudPcFailurePercentage": 8.0
}
```

### <a name="response"></a><span data-ttu-id="81b8f-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b8f-181">Response</span></span>
<span data-ttu-id="81b8f-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81b8f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 528

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "id": "9ecbcf80-cf80-9ecb-80cf-cb9e80cfcb9e",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "virtualNetwork": "Virtual Network value",
  "deviceCount": 11,
  "cloudPcRoundTripTime": 6.666666666666667,
  "cloudPcSignInTime": 5.666666666666667,
  "remoteSignInTime": 5.333333333333333,
  "coreBootTime": 4.0,
  "coreSignInTime": 4.666666666666667,
  "cloudPcFailurePercentage": 8.0
}
```




