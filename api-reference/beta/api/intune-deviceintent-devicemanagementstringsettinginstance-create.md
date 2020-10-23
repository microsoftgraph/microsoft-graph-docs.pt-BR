---
title: Criar deviceManagementStringSettingInstance
description: Criar um novo objeto deviceManagementStringSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dfab9175d9b27f23da00537b28a1db699a6b3cde
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702093"
---
# <a name="create-devicemanagementstringsettinginstance"></a><span data-ttu-id="5f61b-103">Criar deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="5f61b-103">Create deviceManagementStringSettingInstance</span></span>

<span data-ttu-id="5f61b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f61b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f61b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5f61b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f61b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f61b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f61b-107">Criar um novo objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="5f61b-107">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f61b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5f61b-108">Prerequisites</span></span>
<span data-ttu-id="5f61b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f61b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f61b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f61b-111">Permission type</span></span>|<span data-ttu-id="5f61b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5f61b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f61b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f61b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f61b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f61b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5f61b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f61b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f61b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f61b-116">Not supported.</span></span>|
|<span data-ttu-id="5f61b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f61b-117">Application</span></span>|<span data-ttu-id="5f61b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f61b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f61b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f61b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5f61b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f61b-120">Request headers</span></span>
|<span data-ttu-id="5f61b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f61b-121">Header</span></span>|<span data-ttu-id="5f61b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5f61b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f61b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f61b-123">Authorization</span></span>|<span data-ttu-id="5f61b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f61b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f61b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f61b-125">Accept</span></span>|<span data-ttu-id="5f61b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f61b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f61b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f61b-127">Request body</span></span>
<span data-ttu-id="5f61b-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementStringSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="5f61b-128">In the request body, supply a JSON representation for the deviceManagementStringSettingInstance object.</span></span>

<span data-ttu-id="5f61b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementStringSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="5f61b-129">The following table shows the properties that are required when you create the deviceManagementStringSettingInstance.</span></span>

|<span data-ttu-id="5f61b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f61b-130">Property</span></span>|<span data-ttu-id="5f61b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f61b-131">Type</span></span>|<span data-ttu-id="5f61b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f61b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f61b-133">id</span><span class="sxs-lookup"><span data-stu-id="5f61b-133">id</span></span>|<span data-ttu-id="5f61b-134">String</span><span class="sxs-lookup"><span data-stu-id="5f61b-134">String</span></span>|<span data-ttu-id="5f61b-135">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5f61b-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="5f61b-136">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="5f61b-136">definitionId</span></span>|<span data-ttu-id="5f61b-137">String</span><span class="sxs-lookup"><span data-stu-id="5f61b-137">String</span></span>|<span data-ttu-id="5f61b-138">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5f61b-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="5f61b-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="5f61b-139">valueJson</span></span>|<span data-ttu-id="5f61b-140">String</span><span class="sxs-lookup"><span data-stu-id="5f61b-140">String</span></span>|<span data-ttu-id="5f61b-141">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5f61b-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="5f61b-142">value</span><span class="sxs-lookup"><span data-stu-id="5f61b-142">value</span></span>|<span data-ttu-id="5f61b-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f61b-143">String</span></span>|<span data-ttu-id="5f61b-144">O valor da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f61b-144">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="5f61b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f61b-145">Response</span></span>
<span data-ttu-id="5f61b-146">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f61b-146">If successful, this method returns a `201 Created` response code and a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f61b-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f61b-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f61b-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f61b-148">Request</span></span>
<span data-ttu-id="5f61b-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f61b-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5f61b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f61b-150">Response</span></span>
<span data-ttu-id="5f61b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f61b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





