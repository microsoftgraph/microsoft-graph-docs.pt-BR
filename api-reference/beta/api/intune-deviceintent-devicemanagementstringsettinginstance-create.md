---
title: Criar deviceManagementStringSettingInstance
description: Criar um novo objeto deviceManagementStringSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0b9c28944be5c816940fa4f9154bb8411bd0644
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343192"
---
# <a name="create-devicemanagementstringsettinginstance"></a><span data-ttu-id="20542-103">Criar deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="20542-103">Create deviceManagementStringSettingInstance</span></span>

> <span data-ttu-id="20542-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="20542-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20542-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20542-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20542-106">Criar um novo objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="20542-106">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20542-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20542-107">Prerequisites</span></span>
<span data-ttu-id="20542-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20542-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20542-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20542-110">Permission type</span></span>|<span data-ttu-id="20542-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20542-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20542-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20542-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20542-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20542-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="20542-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20542-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20542-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20542-115">Not supported.</span></span>|
|<span data-ttu-id="20542-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20542-116">Application</span></span>|<span data-ttu-id="20542-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20542-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20542-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20542-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="20542-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20542-119">Request headers</span></span>
|<span data-ttu-id="20542-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20542-120">Header</span></span>|<span data-ttu-id="20542-121">Valor</span><span class="sxs-lookup"><span data-stu-id="20542-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20542-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="20542-122">Authorization</span></span>|<span data-ttu-id="20542-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20542-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20542-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20542-124">Accept</span></span>|<span data-ttu-id="20542-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20542-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20542-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20542-126">Request body</span></span>
<span data-ttu-id="20542-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementStringSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="20542-127">In the request body, supply a JSON representation for the deviceManagementStringSettingInstance object.</span></span>

<span data-ttu-id="20542-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementStringSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="20542-128">The following table shows the properties that are required when you create the deviceManagementStringSettingInstance.</span></span>

|<span data-ttu-id="20542-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20542-129">Property</span></span>|<span data-ttu-id="20542-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="20542-130">Type</span></span>|<span data-ttu-id="20542-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="20542-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20542-132">id</span><span class="sxs-lookup"><span data-stu-id="20542-132">id</span></span>|<span data-ttu-id="20542-133">String</span><span class="sxs-lookup"><span data-stu-id="20542-133">String</span></span>|<span data-ttu-id="20542-134">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="20542-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="20542-135">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="20542-135">definitionId</span></span>|<span data-ttu-id="20542-136">String</span><span class="sxs-lookup"><span data-stu-id="20542-136">String</span></span>|<span data-ttu-id="20542-137">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="20542-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="20542-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="20542-138">valueJson</span></span>|<span data-ttu-id="20542-139">String</span><span class="sxs-lookup"><span data-stu-id="20542-139">String</span></span>|<span data-ttu-id="20542-140">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="20542-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="20542-141">value</span><span class="sxs-lookup"><span data-stu-id="20542-141">value</span></span>|<span data-ttu-id="20542-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20542-142">String</span></span>|<span data-ttu-id="20542-143">O valor da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20542-143">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="20542-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="20542-144">Response</span></span>
<span data-ttu-id="20542-145">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20542-145">If successful, this method returns a `201 Created` response code and a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20542-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20542-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="20542-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20542-147">Request</span></span>
<span data-ttu-id="20542-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20542-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="20542-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="20542-149">Response</span></span>
<span data-ttu-id="20542-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20542-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






