---
title: Criar deviceManagementAbstractComplexSettingInstance
description: Criar um novo objeto deviceManagementAbstractComplexSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 722d20f0b9b62218f1a58cb19e29a5d68a5c2d35
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37186250"
---
# <a name="create-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="40edd-103">Criar deviceManagementAbstractComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="40edd-103">Create deviceManagementAbstractComplexSettingInstance</span></span>

> <span data-ttu-id="40edd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40edd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40edd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40edd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40edd-106">Criar um novo objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="40edd-106">Create a new [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40edd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40edd-107">Prerequisites</span></span>
<span data-ttu-id="40edd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40edd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40edd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40edd-110">Permission type</span></span>|<span data-ttu-id="40edd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40edd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40edd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40edd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40edd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40edd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40edd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40edd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40edd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40edd-115">Not supported.</span></span>|
|<span data-ttu-id="40edd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40edd-116">Application</span></span>|<span data-ttu-id="40edd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40edd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40edd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40edd-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="40edd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40edd-119">Request headers</span></span>
|<span data-ttu-id="40edd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40edd-120">Header</span></span>|<span data-ttu-id="40edd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="40edd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40edd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="40edd-122">Authorization</span></span>|<span data-ttu-id="40edd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40edd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40edd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40edd-124">Accept</span></span>|<span data-ttu-id="40edd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40edd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40edd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40edd-126">Request body</span></span>
<span data-ttu-id="40edd-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementAbstractComplexSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="40edd-127">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingInstance object.</span></span>

<span data-ttu-id="40edd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAbstractComplexSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="40edd-128">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingInstance.</span></span>

|<span data-ttu-id="40edd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40edd-129">Property</span></span>|<span data-ttu-id="40edd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="40edd-130">Type</span></span>|<span data-ttu-id="40edd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="40edd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40edd-132">id</span><span class="sxs-lookup"><span data-stu-id="40edd-132">id</span></span>|<span data-ttu-id="40edd-133">String</span><span class="sxs-lookup"><span data-stu-id="40edd-133">String</span></span>|<span data-ttu-id="40edd-134">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="40edd-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="40edd-135">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="40edd-135">definitionId</span></span>|<span data-ttu-id="40edd-136">String</span><span class="sxs-lookup"><span data-stu-id="40edd-136">String</span></span>|<span data-ttu-id="40edd-137">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="40edd-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="40edd-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="40edd-138">valueJson</span></span>|<span data-ttu-id="40edd-139">String</span><span class="sxs-lookup"><span data-stu-id="40edd-139">String</span></span>|<span data-ttu-id="40edd-140">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="40edd-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="40edd-141">implementationid</span><span class="sxs-lookup"><span data-stu-id="40edd-141">implementationId</span></span>|<span data-ttu-id="40edd-142">String</span><span class="sxs-lookup"><span data-stu-id="40edd-142">String</span></span>|<span data-ttu-id="40edd-143">A ID de definição da implementação escolhida dessa configuração complexa</span><span class="sxs-lookup"><span data-stu-id="40edd-143">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="40edd-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="40edd-144">Response</span></span>
<span data-ttu-id="40edd-145">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40edd-145">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40edd-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40edd-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="40edd-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40edd-147">Request</span></span>
<span data-ttu-id="40edd-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40edd-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```

### <a name="response"></a><span data-ttu-id="40edd-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="40edd-149">Response</span></span>
<span data-ttu-id="40edd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40edd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "id": "433e9565-9565-433e-6595-3e4365953e43",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```




