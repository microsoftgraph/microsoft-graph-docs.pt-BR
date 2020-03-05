---
title: Criar deviceManagementBooleanSettingInstance
description: Criar um novo objeto deviceManagementBooleanSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: efb1048ffe3371272efcf6c8c54e366ba42bb2a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42472762"
---
# <a name="create-devicemanagementbooleansettinginstance"></a><span data-ttu-id="6cc98-103">Criar deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="6cc98-103">Create deviceManagementBooleanSettingInstance</span></span>

<span data-ttu-id="6cc98-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6cc98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cc98-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6cc98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cc98-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6cc98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cc98-107">Criar um novo objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="6cc98-107">Create a new [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cc98-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6cc98-108">Prerequisites</span></span>
<span data-ttu-id="6cc98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cc98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cc98-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cc98-111">Permission type</span></span>|<span data-ttu-id="6cc98-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6cc98-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cc98-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cc98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cc98-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cc98-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6cc98-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cc98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cc98-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cc98-116">Not supported.</span></span>|
|<span data-ttu-id="6cc98-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cc98-117">Application</span></span>|<span data-ttu-id="6cc98-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cc98-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cc98-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cc98-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6cc98-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cc98-120">Request headers</span></span>
|<span data-ttu-id="6cc98-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6cc98-121">Header</span></span>|<span data-ttu-id="6cc98-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6cc98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cc98-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cc98-123">Authorization</span></span>|<span data-ttu-id="6cc98-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cc98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cc98-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6cc98-125">Accept</span></span>|<span data-ttu-id="6cc98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cc98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cc98-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cc98-127">Request body</span></span>
<span data-ttu-id="6cc98-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementBooleanSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="6cc98-128">In the request body, supply a JSON representation for the deviceManagementBooleanSettingInstance object.</span></span>

<span data-ttu-id="6cc98-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementBooleanSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="6cc98-129">The following table shows the properties that are required when you create the deviceManagementBooleanSettingInstance.</span></span>

|<span data-ttu-id="6cc98-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cc98-130">Property</span></span>|<span data-ttu-id="6cc98-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cc98-131">Type</span></span>|<span data-ttu-id="6cc98-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cc98-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cc98-133">id</span><span class="sxs-lookup"><span data-stu-id="6cc98-133">id</span></span>|<span data-ttu-id="6cc98-134">String</span><span class="sxs-lookup"><span data-stu-id="6cc98-134">String</span></span>|<span data-ttu-id="6cc98-135">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="6cc98-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="6cc98-136">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="6cc98-136">definitionId</span></span>|<span data-ttu-id="6cc98-137">String</span><span class="sxs-lookup"><span data-stu-id="6cc98-137">String</span></span>|<span data-ttu-id="6cc98-138">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="6cc98-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="6cc98-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="6cc98-139">valueJson</span></span>|<span data-ttu-id="6cc98-140">String</span><span class="sxs-lookup"><span data-stu-id="6cc98-140">String</span></span>|<span data-ttu-id="6cc98-141">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="6cc98-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="6cc98-142">value</span><span class="sxs-lookup"><span data-stu-id="6cc98-142">value</span></span>|<span data-ttu-id="6cc98-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cc98-143">Boolean</span></span>|<span data-ttu-id="6cc98-144">O valor booliano</span><span class="sxs-lookup"><span data-stu-id="6cc98-144">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="6cc98-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cc98-145">Response</span></span>
<span data-ttu-id="6cc98-146">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cc98-146">If successful, this method returns a `201 Created` response code and a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cc98-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cc98-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cc98-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cc98-148">Request</span></span>
<span data-ttu-id="6cc98-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cc98-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6cc98-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cc98-150">Response</span></span>
<span data-ttu-id="6cc98-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cc98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





