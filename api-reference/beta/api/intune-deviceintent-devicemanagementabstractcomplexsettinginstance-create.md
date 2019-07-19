---
title: Criar deviceManagementAbstractComplexSettingInstance
description: Criar um novo objeto deviceManagementAbstractComplexSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34993de09d5a0471b2eaccf2a7b5b421c255fbbd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961032"
---
# <a name="create-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="88f83-103">Criar deviceManagementAbstractComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="88f83-103">Create deviceManagementAbstractComplexSettingInstance</span></span>

> <span data-ttu-id="88f83-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88f83-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88f83-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88f83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88f83-106">Criar um novo objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="88f83-106">Create a new [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88f83-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88f83-107">Prerequisites</span></span>
<span data-ttu-id="88f83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88f83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88f83-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88f83-110">Permission type</span></span>|<span data-ttu-id="88f83-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88f83-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88f83-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88f83-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88f83-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88f83-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88f83-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88f83-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88f83-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88f83-115">Not supported.</span></span>|
|<span data-ttu-id="88f83-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88f83-116">Application</span></span>|<span data-ttu-id="88f83-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88f83-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88f83-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88f83-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="88f83-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88f83-119">Request headers</span></span>
|<span data-ttu-id="88f83-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88f83-120">Header</span></span>|<span data-ttu-id="88f83-121">Valor</span><span class="sxs-lookup"><span data-stu-id="88f83-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88f83-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="88f83-122">Authorization</span></span>|<span data-ttu-id="88f83-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88f83-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88f83-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88f83-124">Accept</span></span>|<span data-ttu-id="88f83-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88f83-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88f83-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88f83-126">Request body</span></span>
<span data-ttu-id="88f83-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementAbstractComplexSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="88f83-127">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingInstance object.</span></span>

<span data-ttu-id="88f83-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAbstractComplexSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="88f83-128">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingInstance.</span></span>

|<span data-ttu-id="88f83-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88f83-129">Property</span></span>|<span data-ttu-id="88f83-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="88f83-130">Type</span></span>|<span data-ttu-id="88f83-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="88f83-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88f83-132">id</span><span class="sxs-lookup"><span data-stu-id="88f83-132">id</span></span>|<span data-ttu-id="88f83-133">String</span><span class="sxs-lookup"><span data-stu-id="88f83-133">String</span></span>|<span data-ttu-id="88f83-134">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="88f83-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="88f83-135">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="88f83-135">definitionId</span></span>|<span data-ttu-id="88f83-136">String</span><span class="sxs-lookup"><span data-stu-id="88f83-136">String</span></span>|<span data-ttu-id="88f83-137">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="88f83-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="88f83-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="88f83-138">valueJson</span></span>|<span data-ttu-id="88f83-139">String</span><span class="sxs-lookup"><span data-stu-id="88f83-139">String</span></span>|<span data-ttu-id="88f83-140">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="88f83-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="88f83-141">implementationid</span><span class="sxs-lookup"><span data-stu-id="88f83-141">implementationId</span></span>|<span data-ttu-id="88f83-142">String</span><span class="sxs-lookup"><span data-stu-id="88f83-142">String</span></span>|<span data-ttu-id="88f83-143">A ID de definição da implementação escolhida dessa configuração complexa</span><span class="sxs-lookup"><span data-stu-id="88f83-143">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="88f83-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="88f83-144">Response</span></span>
<span data-ttu-id="88f83-145">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88f83-145">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88f83-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88f83-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="88f83-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88f83-147">Request</span></span>
<span data-ttu-id="88f83-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88f83-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="88f83-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="88f83-149">Response</span></span>
<span data-ttu-id="88f83-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88f83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





