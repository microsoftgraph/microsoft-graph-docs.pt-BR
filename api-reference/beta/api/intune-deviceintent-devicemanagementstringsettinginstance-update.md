---
title: Atualizar deviceManagementStringSettingInstance
description: Atualiza as propriedades de um objeto deviceManagementStringSettingInstance.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf84fbd078faf49418bdba41beb172adc1aef0c2
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523655"
---
# <a name="update-devicemanagementstringsettinginstance"></a><span data-ttu-id="3c99f-103">Atualizar deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="3c99f-103">Update deviceManagementStringSettingInstance</span></span>

> <span data-ttu-id="3c99f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c99f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c99f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c99f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c99f-106">Atualiza as propriedades de um objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="3c99f-106">Update the properties of a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c99f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c99f-107">Prerequisites</span></span>
<span data-ttu-id="3c99f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c99f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c99f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c99f-110">Permission type</span></span>|<span data-ttu-id="3c99f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c99f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c99f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c99f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c99f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c99f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c99f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c99f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c99f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c99f-115">Not supported.</span></span>|
|<span data-ttu-id="3c99f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c99f-116">Application</span></span>|<span data-ttu-id="3c99f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c99f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c99f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c99f-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="3c99f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c99f-119">Request headers</span></span>
|<span data-ttu-id="3c99f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c99f-120">Header</span></span>|<span data-ttu-id="3c99f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3c99f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c99f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c99f-122">Authorization</span></span>|<span data-ttu-id="3c99f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c99f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c99f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c99f-124">Accept</span></span>|<span data-ttu-id="3c99f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c99f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c99f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c99f-126">Request body</span></span>
<span data-ttu-id="3c99f-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="3c99f-127">In the request body, supply a JSON representation for the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

<span data-ttu-id="3c99f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="3c99f-128">The following table shows the properties that are required when you create the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span></span>

|<span data-ttu-id="3c99f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c99f-129">Property</span></span>|<span data-ttu-id="3c99f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c99f-130">Type</span></span>|<span data-ttu-id="3c99f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c99f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c99f-132">id</span><span class="sxs-lookup"><span data-stu-id="3c99f-132">id</span></span>|<span data-ttu-id="3c99f-133">String</span><span class="sxs-lookup"><span data-stu-id="3c99f-133">String</span></span>|<span data-ttu-id="3c99f-134">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="3c99f-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="3c99f-135">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="3c99f-135">definitionId</span></span>|<span data-ttu-id="3c99f-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3c99f-136">String</span></span>|<span data-ttu-id="3c99f-137">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="3c99f-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="3c99f-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="3c99f-138">valueJson</span></span>|<span data-ttu-id="3c99f-139">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3c99f-139">String</span></span>|<span data-ttu-id="3c99f-140">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="3c99f-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="3c99f-141">value</span><span class="sxs-lookup"><span data-stu-id="3c99f-141">value</span></span>|<span data-ttu-id="3c99f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c99f-142">String</span></span>|<span data-ttu-id="3c99f-143">O valor da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c99f-143">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="3c99f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c99f-144">Response</span></span>
<span data-ttu-id="3c99f-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c99f-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c99f-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c99f-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c99f-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c99f-147">Request</span></span>
<span data-ttu-id="3c99f-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c99f-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="3c99f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c99f-149">Response</span></span>
<span data-ttu-id="3c99f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c99f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```







