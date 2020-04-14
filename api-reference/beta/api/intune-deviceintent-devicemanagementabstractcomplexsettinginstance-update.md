---
title: Atualizar deviceManagementAbstractComplexSettingInstance
description: Atualiza as propriedades de um objeto deviceManagementAbstractComplexSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9fa9188e829931cf25d27e2ca972bd03e364e23
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43330448"
---
# <a name="update-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="fab2f-103">Atualizar deviceManagementAbstractComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="fab2f-103">Update deviceManagementAbstractComplexSettingInstance</span></span>

<span data-ttu-id="fab2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fab2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fab2f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fab2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fab2f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fab2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fab2f-107">Atualiza as propriedades de um objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="fab2f-107">Update the properties of a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fab2f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fab2f-108">Prerequisites</span></span>
<span data-ttu-id="fab2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fab2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fab2f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fab2f-111">Permission type</span></span>|<span data-ttu-id="fab2f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fab2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fab2f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fab2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fab2f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fab2f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fab2f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fab2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fab2f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fab2f-116">Not supported.</span></span>|
|<span data-ttu-id="fab2f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fab2f-117">Application</span></span>|<span data-ttu-id="fab2f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fab2f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fab2f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fab2f-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="fab2f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fab2f-120">Request headers</span></span>
|<span data-ttu-id="fab2f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fab2f-121">Header</span></span>|<span data-ttu-id="fab2f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fab2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fab2f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fab2f-123">Authorization</span></span>|<span data-ttu-id="fab2f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fab2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fab2f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fab2f-125">Accept</span></span>|<span data-ttu-id="fab2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fab2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fab2f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fab2f-127">Request body</span></span>
<span data-ttu-id="fab2f-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="fab2f-128">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="fab2f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="fab2f-129">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="fab2f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fab2f-130">Property</span></span>|<span data-ttu-id="fab2f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fab2f-131">Type</span></span>|<span data-ttu-id="fab2f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fab2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fab2f-133">id</span><span class="sxs-lookup"><span data-stu-id="fab2f-133">id</span></span>|<span data-ttu-id="fab2f-134">String</span><span class="sxs-lookup"><span data-stu-id="fab2f-134">String</span></span>|<span data-ttu-id="fab2f-135">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="fab2f-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="fab2f-136">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="fab2f-136">definitionId</span></span>|<span data-ttu-id="fab2f-137">String</span><span class="sxs-lookup"><span data-stu-id="fab2f-137">String</span></span>|<span data-ttu-id="fab2f-138">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="fab2f-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="fab2f-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="fab2f-139">valueJson</span></span>|<span data-ttu-id="fab2f-140">String</span><span class="sxs-lookup"><span data-stu-id="fab2f-140">String</span></span>|<span data-ttu-id="fab2f-141">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="fab2f-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="fab2f-142">implementationid</span><span class="sxs-lookup"><span data-stu-id="fab2f-142">implementationId</span></span>|<span data-ttu-id="fab2f-143">String</span><span class="sxs-lookup"><span data-stu-id="fab2f-143">String</span></span>|<span data-ttu-id="fab2f-144">A ID de definição da implementação escolhida dessa configuração complexa</span><span class="sxs-lookup"><span data-stu-id="fab2f-144">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="fab2f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="fab2f-145">Response</span></span>
<span data-ttu-id="fab2f-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fab2f-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fab2f-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fab2f-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="fab2f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fab2f-148">Request</span></span>
<span data-ttu-id="fab2f-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fab2f-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fab2f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="fab2f-150">Response</span></span>
<span data-ttu-id="fab2f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fab2f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



