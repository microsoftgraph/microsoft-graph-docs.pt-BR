---
title: Criar deviceManagementIntegerSettingInstance
description: Criar um novo objeto deviceManagementIntegerSettingInstance.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33b2b22d8a1004624a63c9b27e3b25285df9c75f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799794"
---
# <a name="create-devicemanagementintegersettinginstance"></a><span data-ttu-id="2df65-103">Criar deviceManagementIntegerSettingInstance</span><span class="sxs-lookup"><span data-stu-id="2df65-103">Create deviceManagementIntegerSettingInstance</span></span>

> <span data-ttu-id="2df65-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2df65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2df65-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2df65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2df65-106">Criar um novo objeto [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="2df65-106">Create a new [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2df65-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2df65-107">Prerequisites</span></span>
<span data-ttu-id="2df65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2df65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df65-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2df65-110">Permission type</span></span>|<span data-ttu-id="2df65-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2df65-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2df65-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2df65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2df65-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df65-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2df65-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2df65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2df65-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2df65-115">Not supported.</span></span>|
|<span data-ttu-id="2df65-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2df65-116">Application</span></span>|<span data-ttu-id="2df65-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2df65-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2df65-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2df65-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/settings
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="2df65-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2df65-119">Request headers</span></span>
|<span data-ttu-id="2df65-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2df65-120">Header</span></span>|<span data-ttu-id="2df65-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2df65-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2df65-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2df65-122">Authorization</span></span>|<span data-ttu-id="2df65-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2df65-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2df65-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2df65-124">Accept</span></span>|<span data-ttu-id="2df65-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2df65-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2df65-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2df65-126">Request body</span></span>
<span data-ttu-id="2df65-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntegerSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="2df65-127">In the request body, supply a JSON representation for the deviceManagementIntegerSettingInstance object.</span></span>

<span data-ttu-id="2df65-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntegerSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="2df65-128">The following table shows the properties that are required when you create the deviceManagementIntegerSettingInstance.</span></span>

|<span data-ttu-id="2df65-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2df65-129">Property</span></span>|<span data-ttu-id="2df65-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2df65-130">Type</span></span>|<span data-ttu-id="2df65-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2df65-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2df65-132">id</span><span class="sxs-lookup"><span data-stu-id="2df65-132">id</span></span>|<span data-ttu-id="2df65-133">String</span><span class="sxs-lookup"><span data-stu-id="2df65-133">String</span></span>|<span data-ttu-id="2df65-134">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="2df65-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="2df65-135">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="2df65-135">definitionId</span></span>|<span data-ttu-id="2df65-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2df65-136">String</span></span>|<span data-ttu-id="2df65-137">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="2df65-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="2df65-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="2df65-138">valueJson</span></span>|<span data-ttu-id="2df65-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2df65-139">String</span></span>|<span data-ttu-id="2df65-140">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="2df65-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="2df65-141">valor</span><span class="sxs-lookup"><span data-stu-id="2df65-141">value</span></span>|<span data-ttu-id="2df65-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2df65-142">Int32</span></span>|<span data-ttu-id="2df65-143">O valor inteiro</span><span class="sxs-lookup"><span data-stu-id="2df65-143">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="2df65-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df65-144">Response</span></span>
<span data-ttu-id="2df65-145">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2df65-145">If successful, this method returns a `201 Created` response code and a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2df65-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2df65-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="2df65-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2df65-147">Request</span></span>
<span data-ttu-id="2df65-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2df65-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="2df65-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df65-149">Response</span></span>
<span data-ttu-id="2df65-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2df65-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "id": "60468ce7-8ce7-6046-e78c-4660e78c4660",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```





