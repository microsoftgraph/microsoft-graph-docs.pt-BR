---
title: Atualizar deviceManagementBooleanSettingInstance
description: Atualiza as propriedades de um objeto deviceManagementBooleanSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1e19f2d339c82a73d0bf2f0d762673907f72f373
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42472650"
---
# <a name="update-devicemanagementbooleansettinginstance"></a><span data-ttu-id="5462e-103">Atualizar deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="5462e-103">Update deviceManagementBooleanSettingInstance</span></span>

<span data-ttu-id="5462e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5462e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5462e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5462e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5462e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5462e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5462e-107">Atualiza as propriedades de um objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="5462e-107">Update the properties of a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5462e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5462e-108">Prerequisites</span></span>
<span data-ttu-id="5462e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5462e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5462e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5462e-111">Permission type</span></span>|<span data-ttu-id="5462e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5462e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5462e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5462e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5462e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5462e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5462e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5462e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5462e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5462e-116">Not supported.</span></span>|
|<span data-ttu-id="5462e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5462e-117">Application</span></span>|<span data-ttu-id="5462e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5462e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5462e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5462e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5462e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5462e-120">Request headers</span></span>
|<span data-ttu-id="5462e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5462e-121">Header</span></span>|<span data-ttu-id="5462e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5462e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5462e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5462e-123">Authorization</span></span>|<span data-ttu-id="5462e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5462e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5462e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5462e-125">Accept</span></span>|<span data-ttu-id="5462e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5462e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5462e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5462e-127">Request body</span></span>
<span data-ttu-id="5462e-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="5462e-128">In the request body, supply a JSON representation for the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

<span data-ttu-id="5462e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="5462e-129">The following table shows the properties that are required when you create the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span></span>

|<span data-ttu-id="5462e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5462e-130">Property</span></span>|<span data-ttu-id="5462e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5462e-131">Type</span></span>|<span data-ttu-id="5462e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5462e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5462e-133">id</span><span class="sxs-lookup"><span data-stu-id="5462e-133">id</span></span>|<span data-ttu-id="5462e-134">String</span><span class="sxs-lookup"><span data-stu-id="5462e-134">String</span></span>|<span data-ttu-id="5462e-135">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5462e-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="5462e-136">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="5462e-136">definitionId</span></span>|<span data-ttu-id="5462e-137">String</span><span class="sxs-lookup"><span data-stu-id="5462e-137">String</span></span>|<span data-ttu-id="5462e-138">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5462e-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="5462e-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="5462e-139">valueJson</span></span>|<span data-ttu-id="5462e-140">String</span><span class="sxs-lookup"><span data-stu-id="5462e-140">String</span></span>|<span data-ttu-id="5462e-141">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5462e-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="5462e-142">value</span><span class="sxs-lookup"><span data-stu-id="5462e-142">value</span></span>|<span data-ttu-id="5462e-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="5462e-143">Boolean</span></span>|<span data-ttu-id="5462e-144">O valor booliano</span><span class="sxs-lookup"><span data-stu-id="5462e-144">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="5462e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5462e-145">Response</span></span>
<span data-ttu-id="5462e-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5462e-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5462e-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5462e-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="5462e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5462e-148">Request</span></span>
<span data-ttu-id="5462e-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5462e-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5462e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5462e-150">Response</span></span>
<span data-ttu-id="5462e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5462e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





