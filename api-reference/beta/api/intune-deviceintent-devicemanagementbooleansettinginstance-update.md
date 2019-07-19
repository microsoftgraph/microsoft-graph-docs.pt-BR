---
title: Atualizar deviceManagementBooleanSettingInstance
description: Atualiza as propriedades de um objeto deviceManagementBooleanSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab568b8f882487156212805e76c9786948b95d0c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960885"
---
# <a name="update-devicemanagementbooleansettinginstance"></a><span data-ttu-id="5935d-103">Atualizar deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="5935d-103">Update deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="5935d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5935d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5935d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5935d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5935d-106">Atualiza as propriedades de um objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="5935d-106">Update the properties of a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5935d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5935d-107">Prerequisites</span></span>
<span data-ttu-id="5935d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5935d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5935d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5935d-110">Permission type</span></span>|<span data-ttu-id="5935d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5935d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5935d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5935d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5935d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5935d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5935d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5935d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5935d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5935d-115">Not supported.</span></span>|
|<span data-ttu-id="5935d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5935d-116">Application</span></span>|<span data-ttu-id="5935d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5935d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5935d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5935d-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5935d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5935d-119">Request headers</span></span>
|<span data-ttu-id="5935d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5935d-120">Header</span></span>|<span data-ttu-id="5935d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5935d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5935d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5935d-122">Authorization</span></span>|<span data-ttu-id="5935d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5935d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5935d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5935d-124">Accept</span></span>|<span data-ttu-id="5935d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5935d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5935d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5935d-126">Request body</span></span>
<span data-ttu-id="5935d-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="5935d-127">In the request body, supply a JSON representation for the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

<span data-ttu-id="5935d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="5935d-128">The following table shows the properties that are required when you create the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span></span>

|<span data-ttu-id="5935d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5935d-129">Property</span></span>|<span data-ttu-id="5935d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5935d-130">Type</span></span>|<span data-ttu-id="5935d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5935d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5935d-132">id</span><span class="sxs-lookup"><span data-stu-id="5935d-132">id</span></span>|<span data-ttu-id="5935d-133">String</span><span class="sxs-lookup"><span data-stu-id="5935d-133">String</span></span>|<span data-ttu-id="5935d-134">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5935d-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="5935d-135">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="5935d-135">definitionId</span></span>|<span data-ttu-id="5935d-136">String</span><span class="sxs-lookup"><span data-stu-id="5935d-136">String</span></span>|<span data-ttu-id="5935d-137">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5935d-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="5935d-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="5935d-138">valueJson</span></span>|<span data-ttu-id="5935d-139">String</span><span class="sxs-lookup"><span data-stu-id="5935d-139">String</span></span>|<span data-ttu-id="5935d-140">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5935d-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="5935d-141">value</span><span class="sxs-lookup"><span data-stu-id="5935d-141">value</span></span>|<span data-ttu-id="5935d-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="5935d-142">Boolean</span></span>|<span data-ttu-id="5935d-143">O valor booliano</span><span class="sxs-lookup"><span data-stu-id="5935d-143">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="5935d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="5935d-144">Response</span></span>
<span data-ttu-id="5935d-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5935d-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5935d-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5935d-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="5935d-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5935d-147">Request</span></span>
<span data-ttu-id="5935d-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5935d-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 176

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="5935d-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="5935d-149">Response</span></span>
<span data-ttu-id="5935d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5935d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 225

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "id": "bb9b0041-0041-bb9b-4100-9bbb41009bbb",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```





