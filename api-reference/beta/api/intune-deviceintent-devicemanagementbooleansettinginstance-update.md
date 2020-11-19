---
title: Atualizar deviceManagementBooleanSettingInstance
description: Atualiza as propriedades de um objeto deviceManagementBooleanSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 045e23a049dfedd71befdf04ee015d9b10849262
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306293"
---
# <a name="update-devicemanagementbooleansettinginstance"></a><span data-ttu-id="740e0-103">Atualizar deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="740e0-103">Update deviceManagementBooleanSettingInstance</span></span>

<span data-ttu-id="740e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="740e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="740e0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="740e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="740e0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="740e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="740e0-107">Atualiza as propriedades de um objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="740e0-107">Update the properties of a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="740e0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="740e0-108">Prerequisites</span></span>
<span data-ttu-id="740e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="740e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="740e0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="740e0-111">Permission type</span></span>|<span data-ttu-id="740e0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="740e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="740e0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="740e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="740e0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="740e0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="740e0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="740e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="740e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="740e0-116">Not supported.</span></span>|
|<span data-ttu-id="740e0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="740e0-117">Application</span></span>|<span data-ttu-id="740e0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="740e0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="740e0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="740e0-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="740e0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="740e0-120">Request headers</span></span>
|<span data-ttu-id="740e0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="740e0-121">Header</span></span>|<span data-ttu-id="740e0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="740e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="740e0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="740e0-123">Authorization</span></span>|<span data-ttu-id="740e0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="740e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="740e0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="740e0-125">Accept</span></span>|<span data-ttu-id="740e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="740e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="740e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="740e0-127">Request body</span></span>
<span data-ttu-id="740e0-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="740e0-128">In the request body, supply a JSON representation for the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

<span data-ttu-id="740e0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="740e0-129">The following table shows the properties that are required when you create the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span></span>

|<span data-ttu-id="740e0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="740e0-130">Property</span></span>|<span data-ttu-id="740e0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="740e0-131">Type</span></span>|<span data-ttu-id="740e0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="740e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="740e0-133">id</span><span class="sxs-lookup"><span data-stu-id="740e0-133">id</span></span>|<span data-ttu-id="740e0-134">String</span><span class="sxs-lookup"><span data-stu-id="740e0-134">String</span></span>|<span data-ttu-id="740e0-135">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="740e0-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="740e0-136">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="740e0-136">definitionId</span></span>|<span data-ttu-id="740e0-137">String</span><span class="sxs-lookup"><span data-stu-id="740e0-137">String</span></span>|<span data-ttu-id="740e0-138">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="740e0-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="740e0-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="740e0-139">valueJson</span></span>|<span data-ttu-id="740e0-140">String</span><span class="sxs-lookup"><span data-stu-id="740e0-140">String</span></span>|<span data-ttu-id="740e0-141">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="740e0-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="740e0-142">value</span><span class="sxs-lookup"><span data-stu-id="740e0-142">value</span></span>|<span data-ttu-id="740e0-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="740e0-143">Boolean</span></span>|<span data-ttu-id="740e0-144">O valor booliano</span><span class="sxs-lookup"><span data-stu-id="740e0-144">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="740e0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="740e0-145">Response</span></span>
<span data-ttu-id="740e0-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="740e0-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="740e0-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="740e0-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="740e0-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="740e0-148">Request</span></span>
<span data-ttu-id="740e0-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="740e0-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="740e0-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="740e0-150">Response</span></span>
<span data-ttu-id="740e0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="740e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




