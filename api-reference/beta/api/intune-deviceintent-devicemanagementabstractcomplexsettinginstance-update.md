---
title: Atualizar deviceManagementAbstractComplexSettingInstance
description: Atualiza as propriedades de um objeto deviceManagementAbstractComplexSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 57f22c28bbb0710f44178523919f753b08cdec86
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916893"
---
# <a name="update-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="23cfe-103">Atualizar deviceManagementAbstractComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="23cfe-103">Update deviceManagementAbstractComplexSettingInstance</span></span>

> <span data-ttu-id="23cfe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23cfe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23cfe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23cfe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23cfe-106">Atualiza as propriedades de um objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="23cfe-106">Update the properties of a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23cfe-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23cfe-107">Prerequisites</span></span>
<span data-ttu-id="23cfe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23cfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23cfe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23cfe-110">Permission type</span></span>|<span data-ttu-id="23cfe-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23cfe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23cfe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23cfe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23cfe-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23cfe-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23cfe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23cfe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23cfe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23cfe-115">Not supported.</span></span>|
|<span data-ttu-id="23cfe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23cfe-116">Application</span></span>|<span data-ttu-id="23cfe-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23cfe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23cfe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23cfe-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="23cfe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23cfe-119">Request headers</span></span>
|<span data-ttu-id="23cfe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23cfe-120">Header</span></span>|<span data-ttu-id="23cfe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="23cfe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23cfe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="23cfe-122">Authorization</span></span>|<span data-ttu-id="23cfe-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23cfe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23cfe-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23cfe-124">Accept</span></span>|<span data-ttu-id="23cfe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23cfe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23cfe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23cfe-126">Request body</span></span>
<span data-ttu-id="23cfe-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="23cfe-127">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="23cfe-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="23cfe-128">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="23cfe-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23cfe-129">Property</span></span>|<span data-ttu-id="23cfe-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="23cfe-130">Type</span></span>|<span data-ttu-id="23cfe-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="23cfe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23cfe-132">id</span><span class="sxs-lookup"><span data-stu-id="23cfe-132">id</span></span>|<span data-ttu-id="23cfe-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23cfe-133">String</span></span>|<span data-ttu-id="23cfe-134">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="23cfe-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="23cfe-135">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="23cfe-135">definitionId</span></span>|<span data-ttu-id="23cfe-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23cfe-136">String</span></span>|<span data-ttu-id="23cfe-137">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="23cfe-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="23cfe-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="23cfe-138">valueJson</span></span>|<span data-ttu-id="23cfe-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23cfe-139">String</span></span>|<span data-ttu-id="23cfe-140">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="23cfe-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="23cfe-141">implementationid</span><span class="sxs-lookup"><span data-stu-id="23cfe-141">implementationId</span></span>|<span data-ttu-id="23cfe-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23cfe-142">String</span></span>|<span data-ttu-id="23cfe-143">A ID de definição da implementação escolhida dessa configuração complexa</span><span class="sxs-lookup"><span data-stu-id="23cfe-143">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="23cfe-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="23cfe-144">Response</span></span>
<span data-ttu-id="23cfe-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23cfe-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23cfe-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23cfe-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="23cfe-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23cfe-147">Request</span></span>
<span data-ttu-id="23cfe-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23cfe-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```

### <a name="response"></a><span data-ttu-id="23cfe-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="23cfe-149">Response</span></span>
<span data-ttu-id="23cfe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23cfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




