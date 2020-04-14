---
title: Atualizar deviceManagementIntentUserState
description: Atualiza as propriedades de um objeto deviceManagementIntentUserState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fa492e9b758e95c80fae589e70fea823b4ac98f8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43325766"
---
# <a name="update-devicemanagementintentuserstate"></a><span data-ttu-id="b9f7f-103">Atualizar deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="b9f7f-103">Update deviceManagementIntentUserState</span></span>

<span data-ttu-id="b9f7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9f7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9f7f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9f7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9f7f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9f7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9f7f-107">Atualiza as propriedades de um objeto [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="b9f7f-107">Update the properties of a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9f7f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9f7f-108">Prerequisites</span></span>
<span data-ttu-id="b9f7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9f7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9f7f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9f7f-111">Permission type</span></span>|<span data-ttu-id="b9f7f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9f7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9f7f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9f7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9f7f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f7f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9f7f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9f7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9f7f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9f7f-116">Not supported.</span></span>|
|<span data-ttu-id="b9f7f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9f7f-117">Application</span></span>|<span data-ttu-id="b9f7f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f7f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9f7f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9f7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="b9f7f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9f7f-120">Request headers</span></span>
|<span data-ttu-id="b9f7f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9f7f-121">Header</span></span>|<span data-ttu-id="b9f7f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b9f7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9f7f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9f7f-123">Authorization</span></span>|<span data-ttu-id="b9f7f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9f7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9f7f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9f7f-125">Accept</span></span>|<span data-ttu-id="b9f7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9f7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9f7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9f7f-127">Request body</span></span>
<span data-ttu-id="b9f7f-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="b9f7f-128">In the request body, supply a JSON representation for the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

<span data-ttu-id="b9f7f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span><span class="sxs-lookup"><span data-stu-id="b9f7f-129">The following table shows the properties that are required when you create the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span></span>

|<span data-ttu-id="b9f7f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9f7f-130">Property</span></span>|<span data-ttu-id="b9f7f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9f7f-131">Type</span></span>|<span data-ttu-id="b9f7f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9f7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9f7f-133">id</span><span class="sxs-lookup"><span data-stu-id="b9f7f-133">id</span></span>|<span data-ttu-id="b9f7f-134">String</span><span class="sxs-lookup"><span data-stu-id="b9f7f-134">String</span></span>|<span data-ttu-id="b9f7f-135">A ID</span><span class="sxs-lookup"><span data-stu-id="b9f7f-135">The ID</span></span>|
|<span data-ttu-id="b9f7f-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9f7f-136">userPrincipalName</span></span>|<span data-ttu-id="b9f7f-137">String</span><span class="sxs-lookup"><span data-stu-id="b9f7f-137">String</span></span>|<span data-ttu-id="b9f7f-138">O nome principal do usuário que está sendo relatado em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="b9f7f-138">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="b9f7f-139">userName</span><span class="sxs-lookup"><span data-stu-id="b9f7f-139">userName</span></span>|<span data-ttu-id="b9f7f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9f7f-140">String</span></span>|<span data-ttu-id="b9f7f-141">O nome de usuário que está sendo relatado em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="b9f7f-141">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="b9f7f-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="b9f7f-142">deviceCount</span></span>|<span data-ttu-id="b9f7f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b9f7f-143">Int32</span></span>|<span data-ttu-id="b9f7f-144">Contagem de dispositivos que pertencem a um usuário para uma intenção</span><span class="sxs-lookup"><span data-stu-id="b9f7f-144">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="b9f7f-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9f7f-145">lastReportedDateTime</span></span>|<span data-ttu-id="b9f7f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9f7f-146">DateTimeOffset</span></span>|<span data-ttu-id="b9f7f-147">Data e hora da última modificação de um relatório de intenção</span><span class="sxs-lookup"><span data-stu-id="b9f7f-147">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="b9f7f-148">state</span><span class="sxs-lookup"><span data-stu-id="b9f7f-148">state</span></span>|[<span data-ttu-id="b9f7f-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b9f7f-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b9f7f-150">Estado do usuário para uma intenção.</span><span class="sxs-lookup"><span data-stu-id="b9f7f-150">User state for an intent.</span></span> <span data-ttu-id="b9f7f-151">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b9f7f-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="b9f7f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9f7f-152">Response</span></span>
<span data-ttu-id="b9f7f-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9f7f-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9f7f-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9f7f-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9f7f-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9f7f-155">Request</span></span>
<span data-ttu-id="b9f7f-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9f7f-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable"
}
```

### <a name="response"></a><span data-ttu-id="b9f7f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9f7f-157">Response</span></span>
<span data-ttu-id="b9f7f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9f7f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "0201286a-286a-0201-6a28-01026a280102",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable"
}
```



