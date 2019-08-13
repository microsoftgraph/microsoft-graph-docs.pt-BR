---
title: Atualizar securityBaselineDeviceState
description: Atualiza as propriedades de um objeto securityBaselineDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ccbdcacbcc2250b4b55ab3fc4e247dbb4a77512
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349072"
---
# <a name="update-securitybaselinedevicestate"></a><span data-ttu-id="86903-103">Atualizar securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="86903-103">Update securityBaselineDeviceState</span></span>

> <span data-ttu-id="86903-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86903-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86903-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86903-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86903-106">Atualiza as propriedades de um objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="86903-106">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86903-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86903-107">Prerequisites</span></span>
<span data-ttu-id="86903-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86903-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86903-110">Permission type</span></span>|<span data-ttu-id="86903-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86903-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86903-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86903-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86903-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86903-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86903-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86903-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86903-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86903-115">Not supported.</span></span>|
|<span data-ttu-id="86903-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86903-116">Application</span></span>|<span data-ttu-id="86903-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86903-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86903-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86903-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="86903-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86903-119">Request headers</span></span>
|<span data-ttu-id="86903-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86903-120">Header</span></span>|<span data-ttu-id="86903-121">Valor</span><span class="sxs-lookup"><span data-stu-id="86903-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86903-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="86903-122">Authorization</span></span>|<span data-ttu-id="86903-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86903-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86903-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86903-124">Accept</span></span>|<span data-ttu-id="86903-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86903-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86903-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86903-126">Request body</span></span>
<span data-ttu-id="86903-127">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="86903-127">In the request body, supply a JSON representation for the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

<span data-ttu-id="86903-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="86903-128">The following table shows the properties that are required when you create the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>

|<span data-ttu-id="86903-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86903-129">Property</span></span>|<span data-ttu-id="86903-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="86903-130">Type</span></span>|<span data-ttu-id="86903-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="86903-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86903-132">id</span><span class="sxs-lookup"><span data-stu-id="86903-132">id</span></span>|<span data-ttu-id="86903-133">String</span><span class="sxs-lookup"><span data-stu-id="86903-133">String</span></span>|<span data-ttu-id="86903-134">Identificador exclusivo da entidade</span><span class="sxs-lookup"><span data-stu-id="86903-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="86903-135">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="86903-135">managedDeviceId</span></span>|<span data-ttu-id="86903-136">String</span><span class="sxs-lookup"><span data-stu-id="86903-136">String</span></span>|<span data-ttu-id="86903-137">ID de dispositivo do Intune</span><span class="sxs-lookup"><span data-stu-id="86903-137">Intune device id</span></span>|
|<span data-ttu-id="86903-138">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="86903-138">deviceDisplayName</span></span>|<span data-ttu-id="86903-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86903-139">String</span></span>|<span data-ttu-id="86903-140">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="86903-140">Display name of the device</span></span>|
|<span data-ttu-id="86903-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="86903-141">userPrincipalName</span></span>|<span data-ttu-id="86903-142">String</span><span class="sxs-lookup"><span data-stu-id="86903-142">String</span></span>|<span data-ttu-id="86903-143">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="86903-143">User Principal Name</span></span>|
|<span data-ttu-id="86903-144">estado</span><span class="sxs-lookup"><span data-stu-id="86903-144">state</span></span>|[<span data-ttu-id="86903-145">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="86903-145">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="86903-146">Estado de conformidade da linha de base de segurança.</span><span class="sxs-lookup"><span data-stu-id="86903-146">Security baseline compliance state.</span></span> <span data-ttu-id="86903-147">Os possíveis valores são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="86903-147">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="86903-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="86903-148">lastReportedDateTime</span></span>|<span data-ttu-id="86903-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86903-149">DateTimeOffset</span></span>|<span data-ttu-id="86903-150">Data e hora da última modificação do relatório de política</span><span class="sxs-lookup"><span data-stu-id="86903-150">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="86903-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="86903-151">Response</span></span>
<span data-ttu-id="86903-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86903-152">If successful, this method returns a `200 OK` response code and an updated [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86903-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86903-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="86903-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86903-154">Request</span></span>
<span data-ttu-id="86903-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86903-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="86903-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="86903-156">Response</span></span>
<span data-ttu-id="86903-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86903-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






