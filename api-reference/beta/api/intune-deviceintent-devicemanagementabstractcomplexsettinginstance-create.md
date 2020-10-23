---
title: Criar deviceManagementAbstractComplexSettingInstance
description: Criar um novo objeto deviceManagementAbstractComplexSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d20f2a65db92823fd8e10bb261d3469d45fa12b9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732251"
---
# <a name="create-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="7b760-103">Criar deviceManagementAbstractComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="7b760-103">Create deviceManagementAbstractComplexSettingInstance</span></span>

<span data-ttu-id="7b760-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b760-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b760-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7b760-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b760-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b760-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b760-107">Criar um novo objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="7b760-107">Create a new [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b760-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7b760-108">Prerequisites</span></span>
<span data-ttu-id="7b760-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b760-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b760-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b760-111">Permission type</span></span>|<span data-ttu-id="7b760-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7b760-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b760-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b760-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b760-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b760-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b760-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b760-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b760-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b760-116">Not supported.</span></span>|
|<span data-ttu-id="7b760-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b760-117">Application</span></span>|<span data-ttu-id="7b760-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b760-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b760-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b760-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7b760-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b760-120">Request headers</span></span>
|<span data-ttu-id="7b760-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7b760-121">Header</span></span>|<span data-ttu-id="7b760-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7b760-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b760-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b760-123">Authorization</span></span>|<span data-ttu-id="7b760-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b760-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b760-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7b760-125">Accept</span></span>|<span data-ttu-id="7b760-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b760-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b760-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b760-127">Request body</span></span>
<span data-ttu-id="7b760-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementAbstractComplexSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="7b760-128">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingInstance object.</span></span>

<span data-ttu-id="7b760-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAbstractComplexSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="7b760-129">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingInstance.</span></span>

|<span data-ttu-id="7b760-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b760-130">Property</span></span>|<span data-ttu-id="7b760-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b760-131">Type</span></span>|<span data-ttu-id="7b760-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b760-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b760-133">id</span><span class="sxs-lookup"><span data-stu-id="7b760-133">id</span></span>|<span data-ttu-id="7b760-134">String</span><span class="sxs-lookup"><span data-stu-id="7b760-134">String</span></span>|<span data-ttu-id="7b760-135">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="7b760-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="7b760-136">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="7b760-136">definitionId</span></span>|<span data-ttu-id="7b760-137">String</span><span class="sxs-lookup"><span data-stu-id="7b760-137">String</span></span>|<span data-ttu-id="7b760-138">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="7b760-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="7b760-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="7b760-139">valueJson</span></span>|<span data-ttu-id="7b760-140">String</span><span class="sxs-lookup"><span data-stu-id="7b760-140">String</span></span>|<span data-ttu-id="7b760-141">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="7b760-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="7b760-142">implementationid</span><span class="sxs-lookup"><span data-stu-id="7b760-142">implementationId</span></span>|<span data-ttu-id="7b760-143">String</span><span class="sxs-lookup"><span data-stu-id="7b760-143">String</span></span>|<span data-ttu-id="7b760-144">A ID de definição da implementação escolhida dessa configuração complexa</span><span class="sxs-lookup"><span data-stu-id="7b760-144">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="7b760-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b760-145">Response</span></span>
<span data-ttu-id="7b760-146">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b760-146">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b760-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b760-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b760-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b760-148">Request</span></span>
<span data-ttu-id="7b760-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b760-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7b760-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b760-150">Response</span></span>
<span data-ttu-id="7b760-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b760-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





