---
title: Atualizar securityBaselineSettingState
description: Atualiza as propriedades de um objeto securityBaselineSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c65f3c49159f6025ae32ee9a12c7acc395742509
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466123"
---
# <a name="update-securitybaselinesettingstate"></a><span data-ttu-id="d507e-103">Atualizar securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="d507e-103">Update securityBaselineSettingState</span></span>

> <span data-ttu-id="d507e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d507e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d507e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d507e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d507e-106">Atualiza as propriedades de um objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="d507e-106">Update the properties of a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d507e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d507e-107">Prerequisites</span></span>
<span data-ttu-id="d507e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d507e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d507e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d507e-110">Permission type</span></span>|<span data-ttu-id="d507e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d507e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d507e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d507e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d507e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d507e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d507e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d507e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d507e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d507e-115">Not supported.</span></span>|
|<span data-ttu-id="d507e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d507e-116">Application</span></span>|<span data-ttu-id="d507e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d507e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d507e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d507e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d507e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d507e-119">Request headers</span></span>
|<span data-ttu-id="d507e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d507e-120">Header</span></span>|<span data-ttu-id="d507e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d507e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d507e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d507e-122">Authorization</span></span>|<span data-ttu-id="d507e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d507e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d507e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d507e-124">Accept</span></span>|<span data-ttu-id="d507e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d507e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d507e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d507e-126">Request body</span></span>
<span data-ttu-id="d507e-127">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="d507e-127">In the request body, supply a JSON representation for the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>

<span data-ttu-id="d507e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="d507e-128">The following table shows the properties that are required when you create the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span></span>

|<span data-ttu-id="d507e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d507e-129">Property</span></span>|<span data-ttu-id="d507e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d507e-130">Type</span></span>|<span data-ttu-id="d507e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d507e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d507e-132">id</span><span class="sxs-lookup"><span data-stu-id="d507e-132">id</span></span>|<span data-ttu-id="d507e-133">String</span><span class="sxs-lookup"><span data-stu-id="d507e-133">String</span></span>|<span data-ttu-id="d507e-134">Identificador exclusivo da entidade</span><span class="sxs-lookup"><span data-stu-id="d507e-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="d507e-135">settingName</span><span class="sxs-lookup"><span data-stu-id="d507e-135">settingName</span></span>|<span data-ttu-id="d507e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d507e-136">String</span></span>|<span data-ttu-id="d507e-137">O nome da configuração que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d507e-137">The setting name that is being reported</span></span>|
|<span data-ttu-id="d507e-138">state</span><span class="sxs-lookup"><span data-stu-id="d507e-138">state</span></span>|[<span data-ttu-id="d507e-139">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="d507e-139">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="d507e-140">O estado de conformidade da configuração da linha de base de segurança.</span><span class="sxs-lookup"><span data-stu-id="d507e-140">The compliance state of the security baseline setting.</span></span> <span data-ttu-id="d507e-141">Os valores possíveis são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="d507e-141">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="d507e-142">settingCategoryId</span><span class="sxs-lookup"><span data-stu-id="d507e-142">settingCategoryId</span></span>|<span data-ttu-id="d507e-143">String</span><span class="sxs-lookup"><span data-stu-id="d507e-143">String</span></span>|<span data-ttu-id="d507e-144">A ID da categoria de configuração à qual essa configuração pertence</span><span class="sxs-lookup"><span data-stu-id="d507e-144">The setting category id which this setting belongs to</span></span>|



## <a name="response"></a><span data-ttu-id="d507e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d507e-145">Response</span></span>
<span data-ttu-id="d507e-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d507e-146">If successful, this method returns a `200 OK` response code and an updated [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d507e-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d507e-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d507e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d507e-148">Request</span></span>
<span data-ttu-id="d507e-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d507e-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```

### <a name="response"></a><span data-ttu-id="d507e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d507e-150">Response</span></span>
<span data-ttu-id="d507e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d507e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "798e520d-520d-798e-0d52-8e790d528e79",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```



