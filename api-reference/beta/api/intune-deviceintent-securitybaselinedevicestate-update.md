---
title: Atualizar securityBaselineDeviceState
description: Atualiza as propriedades de um objeto securityBaselineDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d783dff194d35bcfa09e1b0f1eef48273df065b2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306069"
---
# <a name="update-securitybaselinedevicestate"></a><span data-ttu-id="aee94-103">Atualizar securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="aee94-103">Update securityBaselineDeviceState</span></span>

<span data-ttu-id="aee94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aee94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aee94-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aee94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aee94-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aee94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aee94-107">Atualiza as propriedades de um objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="aee94-107">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aee94-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aee94-108">Prerequisites</span></span>
<span data-ttu-id="aee94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aee94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aee94-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aee94-111">Permission type</span></span>|<span data-ttu-id="aee94-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aee94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aee94-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aee94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aee94-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aee94-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aee94-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aee94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aee94-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aee94-116">Not supported.</span></span>|
|<span data-ttu-id="aee94-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aee94-117">Application</span></span>|<span data-ttu-id="aee94-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aee94-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aee94-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aee94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="aee94-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aee94-120">Request headers</span></span>
|<span data-ttu-id="aee94-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aee94-121">Header</span></span>|<span data-ttu-id="aee94-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aee94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aee94-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aee94-123">Authorization</span></span>|<span data-ttu-id="aee94-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aee94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aee94-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aee94-125">Accept</span></span>|<span data-ttu-id="aee94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aee94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aee94-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aee94-127">Request body</span></span>
<span data-ttu-id="aee94-128">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="aee94-128">In the request body, supply a JSON representation for the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

<span data-ttu-id="aee94-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="aee94-129">The following table shows the properties that are required when you create the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>

|<span data-ttu-id="aee94-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aee94-130">Property</span></span>|<span data-ttu-id="aee94-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aee94-131">Type</span></span>|<span data-ttu-id="aee94-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aee94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aee94-133">id</span><span class="sxs-lookup"><span data-stu-id="aee94-133">id</span></span>|<span data-ttu-id="aee94-134">String</span><span class="sxs-lookup"><span data-stu-id="aee94-134">String</span></span>|<span data-ttu-id="aee94-135">Identificador exclusivo da entidade</span><span class="sxs-lookup"><span data-stu-id="aee94-135">Unique identifier of the entity</span></span>|
|<span data-ttu-id="aee94-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="aee94-136">managedDeviceId</span></span>|<span data-ttu-id="aee94-137">String</span><span class="sxs-lookup"><span data-stu-id="aee94-137">String</span></span>|<span data-ttu-id="aee94-138">ID de dispositivo do Intune</span><span class="sxs-lookup"><span data-stu-id="aee94-138">Intune device id</span></span>|
|<span data-ttu-id="aee94-139">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="aee94-139">deviceDisplayName</span></span>|<span data-ttu-id="aee94-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aee94-140">String</span></span>|<span data-ttu-id="aee94-141">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="aee94-141">Display name of the device</span></span>|
|<span data-ttu-id="aee94-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aee94-142">userPrincipalName</span></span>|<span data-ttu-id="aee94-143">String</span><span class="sxs-lookup"><span data-stu-id="aee94-143">String</span></span>|<span data-ttu-id="aee94-144">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="aee94-144">User Principal Name</span></span>|
|<span data-ttu-id="aee94-145">state</span><span class="sxs-lookup"><span data-stu-id="aee94-145">state</span></span>|[<span data-ttu-id="aee94-146">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="aee94-146">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="aee94-147">Estado de conformidade da linha de base de segurança.</span><span class="sxs-lookup"><span data-stu-id="aee94-147">Security baseline compliance state.</span></span> <span data-ttu-id="aee94-148">Os possíveis valores são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="aee94-148">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="aee94-149">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="aee94-149">lastReportedDateTime</span></span>|<span data-ttu-id="aee94-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aee94-150">DateTimeOffset</span></span>|<span data-ttu-id="aee94-151">Data e hora da última modificação do relatório de política</span><span class="sxs-lookup"><span data-stu-id="aee94-151">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="aee94-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="aee94-152">Response</span></span>
<span data-ttu-id="aee94-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aee94-153">If successful, this method returns a `200 OK` response code and an updated [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aee94-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aee94-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="aee94-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aee94-155">Request</span></span>
<span data-ttu-id="aee94-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aee94-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aee94-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="aee94-157">Response</span></span>
<span data-ttu-id="aee94-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aee94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




