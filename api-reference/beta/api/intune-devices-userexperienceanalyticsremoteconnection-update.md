---
title: Atualizar userExperienceAnalyticsRemoteConnection
description: Atualize as propriedades de um objeto userExperienceAnalyticsRemoteConnection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6287f070f0bbd610bab40694d3c41fcb6e701a7b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445697"
---
# <a name="update-userexperienceanalyticsremoteconnection"></a><span data-ttu-id="ba1ce-103">Atualizar userExperienceAnalyticsRemoteConnection</span><span class="sxs-lookup"><span data-stu-id="ba1ce-103">Update userExperienceAnalyticsRemoteConnection</span></span>

<span data-ttu-id="ba1ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba1ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba1ce-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba1ce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba1ce-107">Atualize as propriedades de [um objeto userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)</span><span class="sxs-lookup"><span data-stu-id="ba1ce-107">Update the properties of a [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba1ce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba1ce-108">Prerequisites</span></span>
<span data-ttu-id="ba1ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba1ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba1ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba1ce-111">Permission type</span></span>|<span data-ttu-id="ba1ce-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba1ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba1ce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba1ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba1ce-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba1ce-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ba1ce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba1ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba1ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-116">Not supported.</span></span>|
|<span data-ttu-id="ba1ce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba1ce-117">Application</span></span>|<span data-ttu-id="ba1ce-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba1ce-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba1ce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba1ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
```

## <a name="request-headers"></a><span data-ttu-id="ba1ce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba1ce-120">Request headers</span></span>
|<span data-ttu-id="ba1ce-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba1ce-121">Header</span></span>|<span data-ttu-id="ba1ce-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ba1ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba1ce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba1ce-123">Authorization</span></span>|<span data-ttu-id="ba1ce-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba1ce-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba1ce-125">Accept</span></span>|<span data-ttu-id="ba1ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba1ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba1ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba1ce-127">Request body</span></span>
<span data-ttu-id="ba1ce-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)</span><span class="sxs-lookup"><span data-stu-id="ba1ce-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object.</span></span>

<span data-ttu-id="ba1ce-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md).</span><span class="sxs-lookup"><span data-stu-id="ba1ce-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md).</span></span>

|<span data-ttu-id="ba1ce-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba1ce-130">Property</span></span>|<span data-ttu-id="ba1ce-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba1ce-131">Type</span></span>|<span data-ttu-id="ba1ce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba1ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba1ce-133">id</span><span class="sxs-lookup"><span data-stu-id="ba1ce-133">id</span></span>|<span data-ttu-id="ba1ce-134">String</span><span class="sxs-lookup"><span data-stu-id="ba1ce-134">String</span></span>|<span data-ttu-id="ba1ce-135">O identificador exclusivo da entidade de conexão remota de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-135">The unique identifier of the user experience analytics remote connection entity.</span></span>|
|<span data-ttu-id="ba1ce-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="ba1ce-136">deviceId</span></span>|<span data-ttu-id="ba1ce-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba1ce-137">String</span></span>|<span data-ttu-id="ba1ce-138">A id do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-138">The id of the device.</span></span>|
|<span data-ttu-id="ba1ce-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="ba1ce-139">deviceName</span></span>|<span data-ttu-id="ba1ce-140">String</span><span class="sxs-lookup"><span data-stu-id="ba1ce-140">String</span></span>|<span data-ttu-id="ba1ce-141">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-141">The name of the device.</span></span>|
|<span data-ttu-id="ba1ce-142">modelo</span><span class="sxs-lookup"><span data-stu-id="ba1ce-142">model</span></span>|<span data-ttu-id="ba1ce-143">String</span><span class="sxs-lookup"><span data-stu-id="ba1ce-143">String</span></span>|<span data-ttu-id="ba1ce-144">O modelo de dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-144">The user experience analytics device model.</span></span>|
|<span data-ttu-id="ba1ce-145">virtualNetwork</span><span class="sxs-lookup"><span data-stu-id="ba1ce-145">virtualNetwork</span></span>|<span data-ttu-id="ba1ce-146">String</span><span class="sxs-lookup"><span data-stu-id="ba1ce-146">String</span></span>|<span data-ttu-id="ba1ce-147">A rede virtual de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-147">The user experience analytics virtual network.</span></span>|
|<span data-ttu-id="ba1ce-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ba1ce-148">deviceCount</span></span>|<span data-ttu-id="ba1ce-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ba1ce-149">Int32</span></span>|<span data-ttu-id="ba1ce-150">A contagem de conexão remota.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-150">The count of remote connection.</span></span> <span data-ttu-id="ba1ce-151">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="ba1ce-151">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="ba1ce-152">cloudPcRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="ba1ce-152">cloudPcRoundTripTime</span></span>|<span data-ttu-id="ba1ce-153">Duplo</span><span class="sxs-lookup"><span data-stu-id="ba1ce-153">Double</span></span>|<span data-ttu-id="ba1ce-154">O tempo de dica de ida e volta do dispositivo cloud pc.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-154">The round tip time of Cloud PC Device.</span></span> <span data-ttu-id="ba1ce-155">Valores válidos de 0 a 1,79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="ba1ce-155">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="ba1ce-156">cloudPcSignInTime</span><span class="sxs-lookup"><span data-stu-id="ba1ce-156">cloudPcSignInTime</span></span>|<span data-ttu-id="ba1ce-157">Duplo</span><span class="sxs-lookup"><span data-stu-id="ba1ce-157">Double</span></span>|<span data-ttu-id="ba1ce-158">A hora de entrada do dispositivo cloud pc.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-158">The sign in time of Cloud PC Device.</span></span> <span data-ttu-id="ba1ce-159">Valores válidos de 0 a 1,79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="ba1ce-159">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="ba1ce-160">remoteSignInTime</span><span class="sxs-lookup"><span data-stu-id="ba1ce-160">remoteSignInTime</span></span>|<span data-ttu-id="ba1ce-161">Duplo</span><span class="sxs-lookup"><span data-stu-id="ba1ce-161">Double</span></span>|<span data-ttu-id="ba1ce-162">A hora de entrada remota do dispositivo cloud pc.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-162">The remote sign in time of Cloud PC Device.</span></span> <span data-ttu-id="ba1ce-163">Valores válidos de 0 a 1,79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="ba1ce-163">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="ba1ce-164">coreBootTime</span><span class="sxs-lookup"><span data-stu-id="ba1ce-164">coreBootTime</span></span>|<span data-ttu-id="ba1ce-165">Duplo</span><span class="sxs-lookup"><span data-stu-id="ba1ce-165">Double</span></span>|<span data-ttu-id="ba1ce-166">O tempo de inicialização principal do Dispositivo cloud pc.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-166">The core boot time of Cloud PC Device.</span></span> <span data-ttu-id="ba1ce-167">Valores válidos de 0 a 1,79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="ba1ce-167">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="ba1ce-168">coreSignInTime</span><span class="sxs-lookup"><span data-stu-id="ba1ce-168">coreSignInTime</span></span>|<span data-ttu-id="ba1ce-169">Duplo</span><span class="sxs-lookup"><span data-stu-id="ba1ce-169">Double</span></span>|<span data-ttu-id="ba1ce-170">A hora de entrada principal do dispositivo cloud pc.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-170">The core sign in time of Cloud PC Device.</span></span> <span data-ttu-id="ba1ce-171">Valores válidos de 0 a 1,79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="ba1ce-171">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="ba1ce-172">cloudPcFailurePercentage</span><span class="sxs-lookup"><span data-stu-id="ba1ce-172">cloudPcFailurePercentage</span></span>|<span data-ttu-id="ba1ce-173">Duplo</span><span class="sxs-lookup"><span data-stu-id="ba1ce-173">Double</span></span>|<span data-ttu-id="ba1ce-174">A porcentagem de falha de entrada do dispositivo cloud pc.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-174">The sign in failure percentage of Cloud PC Device.</span></span> <span data-ttu-id="ba1ce-175">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="ba1ce-175">Valid values 0 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="ba1ce-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba1ce-176">Response</span></span>
<span data-ttu-id="ba1ce-177">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-177">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba1ce-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba1ce-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba1ce-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba1ce-179">Request</span></span>
<span data-ttu-id="ba1ce-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
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

### <a name="response"></a><span data-ttu-id="ba1ce-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba1ce-181">Response</span></span>
<span data-ttu-id="ba1ce-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba1ce-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




