---
title: Atualizar securityBaselineDeviceState
description: Atualize as propriedades de um objeto securityBaselineDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8890d0ab917c5c916041f7b15abb31fe67ca73b5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154543"
---
# <a name="update-securitybaselinedevicestate"></a><span data-ttu-id="a7be5-103">Atualizar securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="a7be5-103">Update securityBaselineDeviceState</span></span>

<span data-ttu-id="a7be5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7be5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7be5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a7be5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7be5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7be5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7be5-107">Atualize as propriedades de [um objeto securityBaselineDeviceState.](../resources/intune-deviceintent-securitybaselinedevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="a7be5-107">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7be5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7be5-108">Prerequisites</span></span>
<span data-ttu-id="a7be5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7be5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7be5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7be5-111">Permission type</span></span>|<span data-ttu-id="a7be5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7be5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7be5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7be5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7be5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7be5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7be5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7be5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7be5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7be5-116">Not supported.</span></span>|
|<span data-ttu-id="a7be5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7be5-117">Application</span></span>|<span data-ttu-id="a7be5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7be5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7be5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7be5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="a7be5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7be5-120">Request headers</span></span>
|<span data-ttu-id="a7be5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7be5-121">Header</span></span>|<span data-ttu-id="a7be5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a7be5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7be5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7be5-123">Authorization</span></span>|<span data-ttu-id="a7be5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7be5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7be5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a7be5-125">Accept</span></span>|<span data-ttu-id="a7be5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7be5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7be5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7be5-127">Request body</span></span>
<span data-ttu-id="a7be5-128">No corpo da solicitação, fornece uma representação JSON para o [objeto securityBaselineDeviceState.](../resources/intune-deviceintent-securitybaselinedevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="a7be5-128">In the request body, supply a JSON representation for the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

<span data-ttu-id="a7be5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="a7be5-129">The following table shows the properties that are required when you create the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>

|<span data-ttu-id="a7be5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7be5-130">Property</span></span>|<span data-ttu-id="a7be5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7be5-131">Type</span></span>|<span data-ttu-id="a7be5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7be5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7be5-133">id</span><span class="sxs-lookup"><span data-stu-id="a7be5-133">id</span></span>|<span data-ttu-id="a7be5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7be5-134">String</span></span>|<span data-ttu-id="a7be5-135">Identificador exclusivo da entidade</span><span class="sxs-lookup"><span data-stu-id="a7be5-135">Unique identifier of the entity</span></span>|
|<span data-ttu-id="a7be5-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a7be5-136">managedDeviceId</span></span>|<span data-ttu-id="a7be5-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7be5-137">String</span></span>|<span data-ttu-id="a7be5-138">ID de dispositivo do Intune</span><span class="sxs-lookup"><span data-stu-id="a7be5-138">Intune device id</span></span>|
|<span data-ttu-id="a7be5-139">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a7be5-139">deviceDisplayName</span></span>|<span data-ttu-id="a7be5-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7be5-140">String</span></span>|<span data-ttu-id="a7be5-141">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a7be5-141">Display name of the device</span></span>|
|<span data-ttu-id="a7be5-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a7be5-142">userPrincipalName</span></span>|<span data-ttu-id="a7be5-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7be5-143">String</span></span>|<span data-ttu-id="a7be5-144">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="a7be5-144">User Principal Name</span></span>|
|<span data-ttu-id="a7be5-145">state</span><span class="sxs-lookup"><span data-stu-id="a7be5-145">state</span></span>|[<span data-ttu-id="a7be5-146">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="a7be5-146">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="a7be5-147">Estado de conformidade da linha de base de segurança.</span><span class="sxs-lookup"><span data-stu-id="a7be5-147">Security baseline compliance state.</span></span> <span data-ttu-id="a7be5-148">Os possíveis valores são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="a7be5-148">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="a7be5-149">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7be5-149">lastReportedDateTime</span></span>|<span data-ttu-id="a7be5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7be5-150">DateTimeOffset</span></span>|<span data-ttu-id="a7be5-151">Data da última modificação do relatório de política</span><span class="sxs-lookup"><span data-stu-id="a7be5-151">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="a7be5-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7be5-152">Response</span></span>
<span data-ttu-id="a7be5-153">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7be5-153">If successful, this method returns a `200 OK` response code and an updated [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7be5-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7be5-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7be5-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7be5-155">Request</span></span>
<span data-ttu-id="a7be5-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7be5-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a7be5-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7be5-157">Response</span></span>
<span data-ttu-id="a7be5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7be5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




