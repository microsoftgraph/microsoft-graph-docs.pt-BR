---
title: Criar securityBaselineDeviceState
description: Criar um novo objeto securityBaselineDeviceState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72ff5ec9e5215ba4812b3672c10641ec68f06b7b
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522668"
---
# <a name="create-securitybaselinedevicestate"></a><span data-ttu-id="8812d-103">Criar securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="8812d-103">Create securityBaselineDeviceState</span></span>

> <span data-ttu-id="8812d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8812d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8812d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8812d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8812d-106">Criar um novo objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="8812d-106">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8812d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8812d-107">Prerequisites</span></span>
<span data-ttu-id="8812d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8812d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8812d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8812d-110">Permission type</span></span>|<span data-ttu-id="8812d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8812d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8812d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8812d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8812d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8812d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8812d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8812d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8812d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8812d-115">Not supported.</span></span>|
|<span data-ttu-id="8812d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8812d-116">Application</span></span>|<span data-ttu-id="8812d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8812d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8812d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8812d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="8812d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8812d-119">Request headers</span></span>
|<span data-ttu-id="8812d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8812d-120">Header</span></span>|<span data-ttu-id="8812d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8812d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8812d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8812d-122">Authorization</span></span>|<span data-ttu-id="8812d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8812d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8812d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8812d-124">Accept</span></span>|<span data-ttu-id="8812d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8812d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8812d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8812d-126">Request body</span></span>
<span data-ttu-id="8812d-127">No corpo da solicitação, forneça uma representação JSON do objeto securityBaselineDeviceState.</span><span class="sxs-lookup"><span data-stu-id="8812d-127">In the request body, supply a JSON representation for the securityBaselineDeviceState object.</span></span>

<span data-ttu-id="8812d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar securityBaselineDeviceState.</span><span class="sxs-lookup"><span data-stu-id="8812d-128">The following table shows the properties that are required when you create the securityBaselineDeviceState.</span></span>

|<span data-ttu-id="8812d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8812d-129">Property</span></span>|<span data-ttu-id="8812d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8812d-130">Type</span></span>|<span data-ttu-id="8812d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8812d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8812d-132">id</span><span class="sxs-lookup"><span data-stu-id="8812d-132">id</span></span>|<span data-ttu-id="8812d-133">String</span><span class="sxs-lookup"><span data-stu-id="8812d-133">String</span></span>|<span data-ttu-id="8812d-134">Identificador exclusivo da entidade</span><span class="sxs-lookup"><span data-stu-id="8812d-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="8812d-135">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="8812d-135">managedDeviceId</span></span>|<span data-ttu-id="8812d-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8812d-136">String</span></span>|<span data-ttu-id="8812d-137">ID de dispositivo do Intune</span><span class="sxs-lookup"><span data-stu-id="8812d-137">Intune device id</span></span>|
|<span data-ttu-id="8812d-138">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8812d-138">deviceDisplayName</span></span>|<span data-ttu-id="8812d-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8812d-139">String</span></span>|<span data-ttu-id="8812d-140">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8812d-140">Display name of the device</span></span>|
|<span data-ttu-id="8812d-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8812d-141">userPrincipalName</span></span>|<span data-ttu-id="8812d-142">String</span><span class="sxs-lookup"><span data-stu-id="8812d-142">String</span></span>|<span data-ttu-id="8812d-143">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="8812d-143">User Principal Name</span></span>|
|<span data-ttu-id="8812d-144">state</span><span class="sxs-lookup"><span data-stu-id="8812d-144">state</span></span>|[<span data-ttu-id="8812d-145">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="8812d-145">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="8812d-146">Estado de conformidade da linha de base de segurança.</span><span class="sxs-lookup"><span data-stu-id="8812d-146">Security baseline compliance state.</span></span> <span data-ttu-id="8812d-147">Os valores possíveis são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="8812d-147">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="8812d-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8812d-148">lastReportedDateTime</span></span>|<span data-ttu-id="8812d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8812d-149">DateTimeOffset</span></span>|<span data-ttu-id="8812d-150">Data e hora da última modificação do relatório de política</span><span class="sxs-lookup"><span data-stu-id="8812d-150">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="8812d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="8812d-151">Response</span></span>
<span data-ttu-id="8812d-152">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8812d-152">If successful, this method returns a `201 Created` response code and a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8812d-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8812d-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="8812d-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8812d-154">Request</span></span>
<span data-ttu-id="8812d-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8812d-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8812d-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="8812d-156">Response</span></span>
<span data-ttu-id="8812d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8812d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







