---
title: Criar deviceManagementIntentUserState
description: Criar um novo objeto deviceManagementIntentUserState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 932fd37d2460e6e6d0c967e2afb401a1a424fa08
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343444"
---
# <a name="create-devicemanagementintentuserstate"></a><span data-ttu-id="468b0-103">Criar deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="468b0-103">Create deviceManagementIntentUserState</span></span>

> <span data-ttu-id="468b0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="468b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="468b0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="468b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="468b0-106">Criar um novo objeto [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="468b0-106">Create a new [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="468b0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="468b0-107">Prerequisites</span></span>
<span data-ttu-id="468b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="468b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="468b0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="468b0-110">Permission type</span></span>|<span data-ttu-id="468b0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="468b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="468b0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="468b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="468b0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="468b0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="468b0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="468b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="468b0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="468b0-115">Not supported.</span></span>|
|<span data-ttu-id="468b0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="468b0-116">Application</span></span>|<span data-ttu-id="468b0-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="468b0-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="468b0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="468b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/userStates
```

## <a name="request-headers"></a><span data-ttu-id="468b0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="468b0-119">Request headers</span></span>
|<span data-ttu-id="468b0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="468b0-120">Header</span></span>|<span data-ttu-id="468b0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="468b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="468b0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="468b0-122">Authorization</span></span>|<span data-ttu-id="468b0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="468b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="468b0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="468b0-124">Accept</span></span>|<span data-ttu-id="468b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="468b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="468b0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="468b0-126">Request body</span></span>
<span data-ttu-id="468b0-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntentUserState.</span><span class="sxs-lookup"><span data-stu-id="468b0-127">In the request body, supply a JSON representation for the deviceManagementIntentUserState object.</span></span>

<span data-ttu-id="468b0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntentUserState.</span><span class="sxs-lookup"><span data-stu-id="468b0-128">The following table shows the properties that are required when you create the deviceManagementIntentUserState.</span></span>

|<span data-ttu-id="468b0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="468b0-129">Property</span></span>|<span data-ttu-id="468b0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="468b0-130">Type</span></span>|<span data-ttu-id="468b0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="468b0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="468b0-132">id</span><span class="sxs-lookup"><span data-stu-id="468b0-132">id</span></span>|<span data-ttu-id="468b0-133">String</span><span class="sxs-lookup"><span data-stu-id="468b0-133">String</span></span>|<span data-ttu-id="468b0-134">A ID</span><span class="sxs-lookup"><span data-stu-id="468b0-134">The ID</span></span>|
|<span data-ttu-id="468b0-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="468b0-135">userPrincipalName</span></span>|<span data-ttu-id="468b0-136">String</span><span class="sxs-lookup"><span data-stu-id="468b0-136">String</span></span>|<span data-ttu-id="468b0-137">O nome principal do usuário que está sendo relatado em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="468b0-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="468b0-138">userName</span><span class="sxs-lookup"><span data-stu-id="468b0-138">userName</span></span>|<span data-ttu-id="468b0-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="468b0-139">String</span></span>|<span data-ttu-id="468b0-140">O nome de usuário que está sendo relatado em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="468b0-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="468b0-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="468b0-141">deviceCount</span></span>|<span data-ttu-id="468b0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="468b0-142">Int32</span></span>|<span data-ttu-id="468b0-143">Contagem de dispositivos que pertencem a um usuário para uma intenção</span><span class="sxs-lookup"><span data-stu-id="468b0-143">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="468b0-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="468b0-144">lastReportedDateTime</span></span>|<span data-ttu-id="468b0-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="468b0-145">DateTimeOffset</span></span>|<span data-ttu-id="468b0-146">Data e hora da última modificação de um relatório de intenção</span><span class="sxs-lookup"><span data-stu-id="468b0-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="468b0-147">estado</span><span class="sxs-lookup"><span data-stu-id="468b0-147">state</span></span>|[<span data-ttu-id="468b0-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="468b0-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="468b0-149">Estado do usuário para uma intenção.</span><span class="sxs-lookup"><span data-stu-id="468b0-149">User state for an intent.</span></span> <span data-ttu-id="468b0-150">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="468b0-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="468b0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="468b0-151">Response</span></span>
<span data-ttu-id="468b0-152">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="468b0-152">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="468b0-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="468b0-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="468b0-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="468b0-154">Request</span></span>
<span data-ttu-id="468b0-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="468b0-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates
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

### <a name="response"></a><span data-ttu-id="468b0-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="468b0-156">Response</span></span>
<span data-ttu-id="468b0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="468b0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






