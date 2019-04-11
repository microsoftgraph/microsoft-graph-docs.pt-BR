---
title: Criar securityBaselineSettingState
description: Criar um novo objeto securityBaselineSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d4a3a68eaab0f9f4c8b3bb7d4f9e8adf16dea37
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781824"
---
# <a name="create-securitybaselinesettingstate"></a><span data-ttu-id="27338-103">Criar securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="27338-103">Create securityBaselineSettingState</span></span>

> <span data-ttu-id="27338-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27338-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27338-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27338-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27338-106">Criar um novo objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="27338-106">Create a new [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27338-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27338-107">Prerequisites</span></span>
<span data-ttu-id="27338-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27338-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27338-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27338-110">Permission type</span></span>|<span data-ttu-id="27338-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27338-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27338-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27338-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27338-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27338-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27338-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27338-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27338-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27338-115">Not supported.</span></span>|
|<span data-ttu-id="27338-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27338-116">Application</span></span>|<span data-ttu-id="27338-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27338-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27338-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27338-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates
```

## <a name="request-headers"></a><span data-ttu-id="27338-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27338-119">Request headers</span></span>
|<span data-ttu-id="27338-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27338-120">Header</span></span>|<span data-ttu-id="27338-121">Valor</span><span class="sxs-lookup"><span data-stu-id="27338-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27338-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27338-122">Authorization</span></span>|<span data-ttu-id="27338-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27338-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27338-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27338-124">Accept</span></span>|<span data-ttu-id="27338-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27338-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27338-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27338-126">Request body</span></span>
<span data-ttu-id="27338-127">No corpo da solicitação, forneça uma representação JSON do objeto securityBaselineSettingState.</span><span class="sxs-lookup"><span data-stu-id="27338-127">In the request body, supply a JSON representation for the securityBaselineSettingState object.</span></span>

<span data-ttu-id="27338-128">A tabela a seguir mostra as propriedades que são necessárias ao criar securityBaselineSettingState.</span><span class="sxs-lookup"><span data-stu-id="27338-128">The following table shows the properties that are required when you create the securityBaselineSettingState.</span></span>

|<span data-ttu-id="27338-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27338-129">Property</span></span>|<span data-ttu-id="27338-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="27338-130">Type</span></span>|<span data-ttu-id="27338-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="27338-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27338-132">id</span><span class="sxs-lookup"><span data-stu-id="27338-132">id</span></span>|<span data-ttu-id="27338-133">String</span><span class="sxs-lookup"><span data-stu-id="27338-133">String</span></span>|<span data-ttu-id="27338-134">Identificador exclusivo da entidade</span><span class="sxs-lookup"><span data-stu-id="27338-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="27338-135">settingName</span><span class="sxs-lookup"><span data-stu-id="27338-135">settingName</span></span>|<span data-ttu-id="27338-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27338-136">String</span></span>|<span data-ttu-id="27338-137">O nome da configuração que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="27338-137">The setting name that is being reported</span></span>|
|<span data-ttu-id="27338-138">state</span><span class="sxs-lookup"><span data-stu-id="27338-138">state</span></span>|[<span data-ttu-id="27338-139">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="27338-139">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="27338-140">O estado de conformidade da configuração da linha de base de segurança.</span><span class="sxs-lookup"><span data-stu-id="27338-140">The compliance state of the security baseline setting.</span></span> <span data-ttu-id="27338-141">Os valores possíveis são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="27338-141">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="27338-142">settingCategoryId</span><span class="sxs-lookup"><span data-stu-id="27338-142">settingCategoryId</span></span>|<span data-ttu-id="27338-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27338-143">String</span></span>|<span data-ttu-id="27338-144">A ID da categoria de configuração à qual essa configuração pertence</span><span class="sxs-lookup"><span data-stu-id="27338-144">The setting category id which this setting belongs to</span></span>|



## <a name="response"></a><span data-ttu-id="27338-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="27338-145">Response</span></span>
<span data-ttu-id="27338-146">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27338-146">If successful, this method returns a `201 Created` response code and a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27338-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27338-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="27338-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27338-148">Request</span></span>
<span data-ttu-id="27338-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27338-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```

### <a name="response"></a><span data-ttu-id="27338-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="27338-150">Response</span></span>
<span data-ttu-id="27338-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27338-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



