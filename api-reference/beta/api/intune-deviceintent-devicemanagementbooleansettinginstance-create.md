---
title: Criar deviceManagementBooleanSettingInstance
description: Criar um novo objeto deviceManagementBooleanSettingInstance.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0ea64c5c33562cdb2278e0a8b6f9ce00cadb924
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42731093"
---
# <a name="create-devicemanagementbooleansettinginstance"></a><span data-ttu-id="964aa-103">Criar deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="964aa-103">Create deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="964aa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="964aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="964aa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="964aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="964aa-106">Criar um novo objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="964aa-106">Create a new [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="964aa-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="964aa-107">Prerequisites</span></span>
<span data-ttu-id="964aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="964aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="964aa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="964aa-110">Permission type</span></span>|<span data-ttu-id="964aa-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="964aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="964aa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="964aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="964aa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="964aa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="964aa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="964aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="964aa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="964aa-115">Not supported.</span></span>|
|<span data-ttu-id="964aa-116">Application</span><span class="sxs-lookup"><span data-stu-id="964aa-116">Application</span></span>|<span data-ttu-id="964aa-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="964aa-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="964aa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="964aa-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="964aa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="964aa-119">Request headers</span></span>
|<span data-ttu-id="964aa-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="964aa-120">Header</span></span>|<span data-ttu-id="964aa-121">Valor</span><span class="sxs-lookup"><span data-stu-id="964aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="964aa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="964aa-122">Authorization</span></span>|<span data-ttu-id="964aa-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="964aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="964aa-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="964aa-124">Accept</span></span>|<span data-ttu-id="964aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="964aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="964aa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="964aa-126">Request body</span></span>
<span data-ttu-id="964aa-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementBooleanSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="964aa-127">In the request body, supply a JSON representation for the deviceManagementBooleanSettingInstance object.</span></span>

<span data-ttu-id="964aa-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementBooleanSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="964aa-128">The following table shows the properties that are required when you create the deviceManagementBooleanSettingInstance.</span></span>

|<span data-ttu-id="964aa-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="964aa-129">Property</span></span>|<span data-ttu-id="964aa-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="964aa-130">Type</span></span>|<span data-ttu-id="964aa-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="964aa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="964aa-132">id</span><span class="sxs-lookup"><span data-stu-id="964aa-132">id</span></span>|<span data-ttu-id="964aa-133">String</span><span class="sxs-lookup"><span data-stu-id="964aa-133">String</span></span>|<span data-ttu-id="964aa-134">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="964aa-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="964aa-135">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="964aa-135">definitionId</span></span>|<span data-ttu-id="964aa-136">String</span><span class="sxs-lookup"><span data-stu-id="964aa-136">String</span></span>|<span data-ttu-id="964aa-137">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="964aa-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="964aa-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="964aa-138">valueJson</span></span>|<span data-ttu-id="964aa-139">String</span><span class="sxs-lookup"><span data-stu-id="964aa-139">String</span></span>|<span data-ttu-id="964aa-140">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="964aa-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="964aa-141">value</span><span class="sxs-lookup"><span data-stu-id="964aa-141">value</span></span>|<span data-ttu-id="964aa-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="964aa-142">Boolean</span></span>|<span data-ttu-id="964aa-143">O valor booliano</span><span class="sxs-lookup"><span data-stu-id="964aa-143">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="964aa-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="964aa-144">Response</span></span>
<span data-ttu-id="964aa-145">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="964aa-145">If successful, this method returns a `201 Created` response code and a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="964aa-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="964aa-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="964aa-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="964aa-147">Request</span></span>
<span data-ttu-id="964aa-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="964aa-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 176

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="964aa-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="964aa-149">Response</span></span>
<span data-ttu-id="964aa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="964aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




