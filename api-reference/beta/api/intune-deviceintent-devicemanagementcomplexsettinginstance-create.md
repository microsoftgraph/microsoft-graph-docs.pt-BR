---
title: Criar deviceManagementComplexSettingInstance
description: Criar um novo objeto deviceManagementComplexSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd7cc4a8775a66fdc258dcf33f30cd6de2289ee0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343808"
---
# <a name="create-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="27aa8-103">Criar deviceManagementComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="27aa8-103">Create deviceManagementComplexSettingInstance</span></span>

> <span data-ttu-id="27aa8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27aa8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27aa8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27aa8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27aa8-106">Criar um novo objeto [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="27aa8-106">Create a new [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27aa8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27aa8-107">Prerequisites</span></span>
<span data-ttu-id="27aa8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27aa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27aa8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27aa8-110">Permission type</span></span>|<span data-ttu-id="27aa8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27aa8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27aa8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27aa8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27aa8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27aa8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27aa8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27aa8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27aa8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27aa8-115">Not supported.</span></span>|
|<span data-ttu-id="27aa8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27aa8-116">Application</span></span>|<span data-ttu-id="27aa8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27aa8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27aa8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27aa8-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="27aa8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27aa8-119">Request headers</span></span>
|<span data-ttu-id="27aa8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27aa8-120">Header</span></span>|<span data-ttu-id="27aa8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="27aa8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27aa8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27aa8-122">Authorization</span></span>|<span data-ttu-id="27aa8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27aa8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27aa8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27aa8-124">Accept</span></span>|<span data-ttu-id="27aa8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27aa8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27aa8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27aa8-126">Request body</span></span>
<span data-ttu-id="27aa8-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementComplexSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="27aa8-127">In the request body, supply a JSON representation for the deviceManagementComplexSettingInstance object.</span></span>

<span data-ttu-id="27aa8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementComplexSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="27aa8-128">The following table shows the properties that are required when you create the deviceManagementComplexSettingInstance.</span></span>

|<span data-ttu-id="27aa8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27aa8-129">Property</span></span>|<span data-ttu-id="27aa8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="27aa8-130">Type</span></span>|<span data-ttu-id="27aa8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="27aa8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27aa8-132">id</span><span class="sxs-lookup"><span data-stu-id="27aa8-132">id</span></span>|<span data-ttu-id="27aa8-133">String</span><span class="sxs-lookup"><span data-stu-id="27aa8-133">String</span></span>|<span data-ttu-id="27aa8-134">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="27aa8-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="27aa8-135">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="27aa8-135">definitionId</span></span>|<span data-ttu-id="27aa8-136">String</span><span class="sxs-lookup"><span data-stu-id="27aa8-136">String</span></span>|<span data-ttu-id="27aa8-137">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="27aa8-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="27aa8-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="27aa8-138">valueJson</span></span>|<span data-ttu-id="27aa8-139">String</span><span class="sxs-lookup"><span data-stu-id="27aa8-139">String</span></span>|<span data-ttu-id="27aa8-140">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="27aa8-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="27aa8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="27aa8-141">Response</span></span>
<span data-ttu-id="27aa8-142">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27aa8-142">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27aa8-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27aa8-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="27aa8-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27aa8-144">Request</span></span>
<span data-ttu-id="27aa8-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27aa8-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="27aa8-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="27aa8-146">Response</span></span>
<span data-ttu-id="27aa8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27aa8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 207

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```






