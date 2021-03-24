---
title: Criar deviceManagementIntegerSettingInstance
description: Crie um novo objeto deviceManagementIntegerSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d6948766b10001b92e58d14d3191151dd8281c64
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127113"
---
# <a name="create-devicemanagementintegersettinginstance"></a><span data-ttu-id="8444a-103">Criar deviceManagementIntegerSettingInstance</span><span class="sxs-lookup"><span data-stu-id="8444a-103">Create deviceManagementIntegerSettingInstance</span></span>

<span data-ttu-id="8444a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8444a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8444a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8444a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8444a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8444a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8444a-107">Crie um novo [objeto deviceManagementIntegerSettingInstance.](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="8444a-107">Create a new [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8444a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8444a-108">Prerequisites</span></span>
<span data-ttu-id="8444a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8444a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8444a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8444a-111">Permission type</span></span>|<span data-ttu-id="8444a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8444a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8444a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8444a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8444a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8444a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8444a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8444a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8444a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8444a-116">Not supported.</span></span>|
|<span data-ttu-id="8444a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8444a-117">Application</span></span>|<span data-ttu-id="8444a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8444a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8444a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8444a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="8444a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8444a-120">Request headers</span></span>
|<span data-ttu-id="8444a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8444a-121">Header</span></span>|<span data-ttu-id="8444a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8444a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8444a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8444a-123">Authorization</span></span>|<span data-ttu-id="8444a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8444a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8444a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8444a-125">Accept</span></span>|<span data-ttu-id="8444a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8444a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8444a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8444a-127">Request body</span></span>
<span data-ttu-id="8444a-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementIntegerSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="8444a-128">In the request body, supply a JSON representation for the deviceManagementIntegerSettingInstance object.</span></span>

<span data-ttu-id="8444a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntegerSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="8444a-129">The following table shows the properties that are required when you create the deviceManagementIntegerSettingInstance.</span></span>

|<span data-ttu-id="8444a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8444a-130">Property</span></span>|<span data-ttu-id="8444a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8444a-131">Type</span></span>|<span data-ttu-id="8444a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8444a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8444a-133">id</span><span class="sxs-lookup"><span data-stu-id="8444a-133">id</span></span>|<span data-ttu-id="8444a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8444a-134">String</span></span>|<span data-ttu-id="8444a-135">A ID da instância de configuração Herdada [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="8444a-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="8444a-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="8444a-136">definitionId</span></span>|<span data-ttu-id="8444a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8444a-137">String</span></span>|<span data-ttu-id="8444a-138">A ID da definição de configuração para esta instância Herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="8444a-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="8444a-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="8444a-139">valueJson</span></span>|<span data-ttu-id="8444a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8444a-140">String</span></span>|<span data-ttu-id="8444a-141">Representação JSON do valor Herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="8444a-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="8444a-142">valor</span><span class="sxs-lookup"><span data-stu-id="8444a-142">value</span></span>|<span data-ttu-id="8444a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8444a-143">Int32</span></span>|<span data-ttu-id="8444a-144">O valor inteiro</span><span class="sxs-lookup"><span data-stu-id="8444a-144">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="8444a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8444a-145">Response</span></span>
<span data-ttu-id="8444a-146">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8444a-146">If successful, this method returns a `201 Created` response code and a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8444a-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8444a-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="8444a-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8444a-148">Request</span></span>
<span data-ttu-id="8444a-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8444a-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8444a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8444a-150">Response</span></span>
<span data-ttu-id="8444a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8444a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




