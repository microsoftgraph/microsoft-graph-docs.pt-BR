---
title: Atualizar deviceManagementIntegerSettingInstance
description: Atualiza as propriedades de um objeto deviceManagementIntegerSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2381cd3a0b9c8acc67388ce12180c3a436d9e20
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707378"
---
# <a name="update-devicemanagementintegersettinginstance"></a><span data-ttu-id="81a93-103">Atualizar deviceManagementIntegerSettingInstance</span><span class="sxs-lookup"><span data-stu-id="81a93-103">Update deviceManagementIntegerSettingInstance</span></span>

<span data-ttu-id="81a93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81a93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81a93-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81a93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81a93-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81a93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81a93-107">Atualiza as propriedades de um objeto [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="81a93-107">Update the properties of a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81a93-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81a93-108">Prerequisites</span></span>
<span data-ttu-id="81a93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81a93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81a93-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81a93-111">Permission type</span></span>|<span data-ttu-id="81a93-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81a93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81a93-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81a93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81a93-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81a93-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="81a93-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81a93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81a93-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81a93-116">Not supported.</span></span>|
|<span data-ttu-id="81a93-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81a93-117">Application</span></span>|<span data-ttu-id="81a93-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81a93-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81a93-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81a93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="request-headers"></a><span data-ttu-id="81a93-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81a93-120">Request headers</span></span>
|<span data-ttu-id="81a93-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81a93-121">Header</span></span>|<span data-ttu-id="81a93-122">Valor</span><span class="sxs-lookup"><span data-stu-id="81a93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81a93-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="81a93-123">Authorization</span></span>|<span data-ttu-id="81a93-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81a93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81a93-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81a93-125">Accept</span></span>|<span data-ttu-id="81a93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81a93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81a93-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81a93-127">Request body</span></span>
<span data-ttu-id="81a93-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="81a93-128">In the request body, supply a JSON representation for the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

<span data-ttu-id="81a93-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="81a93-129">The following table shows the properties that are required when you create the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span></span>

|<span data-ttu-id="81a93-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81a93-130">Property</span></span>|<span data-ttu-id="81a93-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="81a93-131">Type</span></span>|<span data-ttu-id="81a93-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="81a93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81a93-133">id</span><span class="sxs-lookup"><span data-stu-id="81a93-133">id</span></span>|<span data-ttu-id="81a93-134">String</span><span class="sxs-lookup"><span data-stu-id="81a93-134">String</span></span>|<span data-ttu-id="81a93-135">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="81a93-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="81a93-136">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="81a93-136">definitionId</span></span>|<span data-ttu-id="81a93-137">String</span><span class="sxs-lookup"><span data-stu-id="81a93-137">String</span></span>|<span data-ttu-id="81a93-138">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="81a93-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="81a93-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="81a93-139">valueJson</span></span>|<span data-ttu-id="81a93-140">String</span><span class="sxs-lookup"><span data-stu-id="81a93-140">String</span></span>|<span data-ttu-id="81a93-141">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="81a93-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="81a93-142">valor</span><span class="sxs-lookup"><span data-stu-id="81a93-142">value</span></span>|<span data-ttu-id="81a93-143">Int32</span><span class="sxs-lookup"><span data-stu-id="81a93-143">Int32</span></span>|<span data-ttu-id="81a93-144">O valor inteiro</span><span class="sxs-lookup"><span data-stu-id="81a93-144">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="81a93-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="81a93-145">Response</span></span>
<span data-ttu-id="81a93-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81a93-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81a93-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81a93-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="81a93-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81a93-148">Request</span></span>
<span data-ttu-id="81a93-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81a93-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="81a93-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="81a93-150">Response</span></span>
<span data-ttu-id="81a93-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81a93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





