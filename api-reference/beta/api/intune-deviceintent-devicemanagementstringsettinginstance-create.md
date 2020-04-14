---
title: Criar deviceManagementStringSettingInstance
description: Criar um novo objeto deviceManagementStringSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f4f52a8bfe2087594da5d8da98e9cac0ca56a2fe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43325254"
---
# <a name="create-devicemanagementstringsettinginstance"></a><span data-ttu-id="01748-103">Criar deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="01748-103">Create deviceManagementStringSettingInstance</span></span>

<span data-ttu-id="01748-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01748-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01748-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01748-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01748-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01748-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01748-107">Criar um novo objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="01748-107">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01748-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01748-108">Prerequisites</span></span>
<span data-ttu-id="01748-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01748-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01748-111">Permission type</span></span>|<span data-ttu-id="01748-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01748-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01748-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01748-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01748-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01748-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01748-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01748-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01748-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01748-116">Not supported.</span></span>|
|<span data-ttu-id="01748-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01748-117">Application</span></span>|<span data-ttu-id="01748-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01748-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01748-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01748-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="01748-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01748-120">Request headers</span></span>
|<span data-ttu-id="01748-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01748-121">Header</span></span>|<span data-ttu-id="01748-122">Valor</span><span class="sxs-lookup"><span data-stu-id="01748-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01748-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="01748-123">Authorization</span></span>|<span data-ttu-id="01748-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01748-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01748-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01748-125">Accept</span></span>|<span data-ttu-id="01748-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01748-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01748-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01748-127">Request body</span></span>
<span data-ttu-id="01748-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementStringSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="01748-128">In the request body, supply a JSON representation for the deviceManagementStringSettingInstance object.</span></span>

<span data-ttu-id="01748-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementStringSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="01748-129">The following table shows the properties that are required when you create the deviceManagementStringSettingInstance.</span></span>

|<span data-ttu-id="01748-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01748-130">Property</span></span>|<span data-ttu-id="01748-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="01748-131">Type</span></span>|<span data-ttu-id="01748-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="01748-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01748-133">id</span><span class="sxs-lookup"><span data-stu-id="01748-133">id</span></span>|<span data-ttu-id="01748-134">String</span><span class="sxs-lookup"><span data-stu-id="01748-134">String</span></span>|<span data-ttu-id="01748-135">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="01748-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="01748-136">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="01748-136">definitionId</span></span>|<span data-ttu-id="01748-137">String</span><span class="sxs-lookup"><span data-stu-id="01748-137">String</span></span>|<span data-ttu-id="01748-138">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="01748-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="01748-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="01748-139">valueJson</span></span>|<span data-ttu-id="01748-140">String</span><span class="sxs-lookup"><span data-stu-id="01748-140">String</span></span>|<span data-ttu-id="01748-141">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="01748-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="01748-142">value</span><span class="sxs-lookup"><span data-stu-id="01748-142">value</span></span>|<span data-ttu-id="01748-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01748-143">String</span></span>|<span data-ttu-id="01748-144">O valor da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01748-144">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="01748-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="01748-145">Response</span></span>
<span data-ttu-id="01748-146">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01748-146">If successful, this method returns a `201 Created` response code and a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01748-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01748-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="01748-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01748-148">Request</span></span>
<span data-ttu-id="01748-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01748-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="01748-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="01748-150">Response</span></span>
<span data-ttu-id="01748-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01748-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



