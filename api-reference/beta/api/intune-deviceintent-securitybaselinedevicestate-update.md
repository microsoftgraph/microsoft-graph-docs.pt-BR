---
title: Atualizar securityBaselineDeviceState
description: Atualiza as propriedades de um objeto securityBaselineDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e36f5ec306b0230e148ac4970dd0011b934d030
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179464"
---
# <a name="update-securitybaselinedevicestate"></a><span data-ttu-id="d7aab-103">Atualizar securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="d7aab-103">Update securityBaselineDeviceState</span></span>

> <span data-ttu-id="d7aab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7aab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7aab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7aab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7aab-106">Atualiza as propriedades de um objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="d7aab-106">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7aab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7aab-107">Prerequisites</span></span>
<span data-ttu-id="d7aab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7aab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7aab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7aab-110">Permission type</span></span>|<span data-ttu-id="d7aab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7aab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7aab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7aab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7aab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7aab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7aab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7aab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7aab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7aab-115">Not supported.</span></span>|
|<span data-ttu-id="d7aab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7aab-116">Application</span></span>|<span data-ttu-id="d7aab-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7aab-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7aab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7aab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d7aab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7aab-119">Request headers</span></span>
|<span data-ttu-id="d7aab-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7aab-120">Header</span></span>|<span data-ttu-id="d7aab-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d7aab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7aab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7aab-122">Authorization</span></span>|<span data-ttu-id="d7aab-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7aab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7aab-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7aab-124">Accept</span></span>|<span data-ttu-id="d7aab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7aab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7aab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7aab-126">Request body</span></span>
<span data-ttu-id="d7aab-127">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="d7aab-127">In the request body, supply a JSON representation for the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

<span data-ttu-id="d7aab-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="d7aab-128">The following table shows the properties that are required when you create the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>

|<span data-ttu-id="d7aab-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7aab-129">Property</span></span>|<span data-ttu-id="d7aab-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7aab-130">Type</span></span>|<span data-ttu-id="d7aab-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7aab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7aab-132">id</span><span class="sxs-lookup"><span data-stu-id="d7aab-132">id</span></span>|<span data-ttu-id="d7aab-133">String</span><span class="sxs-lookup"><span data-stu-id="d7aab-133">String</span></span>|<span data-ttu-id="d7aab-134">Identificador exclusivo da entidade</span><span class="sxs-lookup"><span data-stu-id="d7aab-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="d7aab-135">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d7aab-135">managedDeviceId</span></span>|<span data-ttu-id="d7aab-136">String</span><span class="sxs-lookup"><span data-stu-id="d7aab-136">String</span></span>|<span data-ttu-id="d7aab-137">ID de dispositivo do Intune</span><span class="sxs-lookup"><span data-stu-id="d7aab-137">Intune device id</span></span>|
|<span data-ttu-id="d7aab-138">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d7aab-138">deviceDisplayName</span></span>|<span data-ttu-id="d7aab-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7aab-139">String</span></span>|<span data-ttu-id="d7aab-140">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d7aab-140">Display name of the device</span></span>|
|<span data-ttu-id="d7aab-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d7aab-141">userPrincipalName</span></span>|<span data-ttu-id="d7aab-142">String</span><span class="sxs-lookup"><span data-stu-id="d7aab-142">String</span></span>|<span data-ttu-id="d7aab-143">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="d7aab-143">User Principal Name</span></span>|
|<span data-ttu-id="d7aab-144">estado</span><span class="sxs-lookup"><span data-stu-id="d7aab-144">state</span></span>|[<span data-ttu-id="d7aab-145">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="d7aab-145">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="d7aab-146">Estado de conformidade da linha de base de segurança.</span><span class="sxs-lookup"><span data-stu-id="d7aab-146">Security baseline compliance state.</span></span> <span data-ttu-id="d7aab-147">Os possíveis valores são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="d7aab-147">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="d7aab-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7aab-148">lastReportedDateTime</span></span>|<span data-ttu-id="d7aab-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7aab-149">DateTimeOffset</span></span>|<span data-ttu-id="d7aab-150">Data e hora da última modificação do relatório de política</span><span class="sxs-lookup"><span data-stu-id="d7aab-150">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="d7aab-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7aab-151">Response</span></span>
<span data-ttu-id="d7aab-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7aab-152">If successful, this method returns a `200 OK` response code and an updated [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7aab-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7aab-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7aab-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7aab-154">Request</span></span>
<span data-ttu-id="d7aab-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7aab-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
Content-type: application/json
Content-length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "managedDeviceId": "Managed Device Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "state": "secure",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="d7aab-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7aab-156">Response</span></span>
<span data-ttu-id="d7aab-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7aab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "id": "182749bf-49bf-1827-bf49-2718bf492718",
  "managedDeviceId": "Managed Device Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "state": "secure",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```




