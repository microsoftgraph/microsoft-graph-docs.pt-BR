---
title: Criar securityBaselineDeviceState
description: Criar um novo objeto securityBaselineDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2b0ab267da75b76d66302e5e621c9030917d5c85
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945386"
---
# <a name="create-securitybaselinedevicestate"></a><span data-ttu-id="ed690-103">Criar securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="ed690-103">Create securityBaselineDeviceState</span></span>

> <span data-ttu-id="ed690-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed690-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed690-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed690-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed690-106">Criar um novo objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="ed690-106">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed690-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed690-107">Prerequisites</span></span>
<span data-ttu-id="ed690-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed690-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed690-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed690-110">Permission type</span></span>|<span data-ttu-id="ed690-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed690-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed690-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed690-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed690-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed690-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed690-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed690-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed690-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed690-115">Not supported.</span></span>|
|<span data-ttu-id="ed690-116">Application</span><span class="sxs-lookup"><span data-stu-id="ed690-116">Application</span></span>|<span data-ttu-id="ed690-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed690-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed690-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed690-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="ed690-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed690-119">Request headers</span></span>
|<span data-ttu-id="ed690-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed690-120">Header</span></span>|<span data-ttu-id="ed690-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ed690-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed690-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed690-122">Authorization</span></span>|<span data-ttu-id="ed690-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed690-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed690-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed690-124">Accept</span></span>|<span data-ttu-id="ed690-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed690-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed690-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed690-126">Request body</span></span>
<span data-ttu-id="ed690-127">No corpo da solicitação, forneça uma representação JSON do objeto securityBaselineDeviceState.</span><span class="sxs-lookup"><span data-stu-id="ed690-127">In the request body, supply a JSON representation for the securityBaselineDeviceState object.</span></span>

<span data-ttu-id="ed690-128">A tabela a seguir mostra as propriedades que são necessárias ao criar securityBaselineDeviceState.</span><span class="sxs-lookup"><span data-stu-id="ed690-128">The following table shows the properties that are required when you create the securityBaselineDeviceState.</span></span>

|<span data-ttu-id="ed690-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed690-129">Property</span></span>|<span data-ttu-id="ed690-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed690-130">Type</span></span>|<span data-ttu-id="ed690-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed690-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed690-132">id</span><span class="sxs-lookup"><span data-stu-id="ed690-132">id</span></span>|<span data-ttu-id="ed690-133">String</span><span class="sxs-lookup"><span data-stu-id="ed690-133">String</span></span>|<span data-ttu-id="ed690-134">Identificador exclusivo da entidade</span><span class="sxs-lookup"><span data-stu-id="ed690-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="ed690-135">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="ed690-135">managedDeviceId</span></span>|<span data-ttu-id="ed690-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="ed690-136">String</span></span>|<span data-ttu-id="ed690-137">ID de dispositivo do Intune</span><span class="sxs-lookup"><span data-stu-id="ed690-137">Intune device id</span></span>|
|<span data-ttu-id="ed690-138">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ed690-138">deviceDisplayName</span></span>|<span data-ttu-id="ed690-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed690-139">String</span></span>|<span data-ttu-id="ed690-140">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ed690-140">Display name of the device</span></span>|
|<span data-ttu-id="ed690-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ed690-141">userPrincipalName</span></span>|<span data-ttu-id="ed690-142">String</span><span class="sxs-lookup"><span data-stu-id="ed690-142">String</span></span>|<span data-ttu-id="ed690-143">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="ed690-143">User Principal Name</span></span>|
|<span data-ttu-id="ed690-144">state</span><span class="sxs-lookup"><span data-stu-id="ed690-144">state</span></span>|[<span data-ttu-id="ed690-145">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="ed690-145">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="ed690-146">Estado de conformidade da linha de base de segurança.</span><span class="sxs-lookup"><span data-stu-id="ed690-146">Security baseline compliance state.</span></span> <span data-ttu-id="ed690-147">Os possíveis valores são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="ed690-147">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="ed690-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed690-148">lastReportedDateTime</span></span>|<span data-ttu-id="ed690-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed690-149">DateTimeOffset</span></span>|<span data-ttu-id="ed690-150">Data e hora da última modificação do relatório de política</span><span class="sxs-lookup"><span data-stu-id="ed690-150">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="ed690-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed690-151">Response</span></span>
<span data-ttu-id="ed690-152">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed690-152">If successful, this method returns a `201 Created` response code and a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed690-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed690-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed690-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed690-154">Request</span></span>
<span data-ttu-id="ed690-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed690-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
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

### <a name="response"></a><span data-ttu-id="ed690-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed690-156">Response</span></span>
<span data-ttu-id="ed690-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed690-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





