---
title: Atualizar deviceManagementAbstractComplexSettingInstance
description: Atualize as propriedades de um objeto deviceManagementAbstractComplexSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a5c6040e4a8c1e8c0bfd2504bf395fcd3db82146
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146682"
---
# <a name="update-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="d03d8-103">Atualizar deviceManagementAbstractComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="d03d8-103">Update deviceManagementAbstractComplexSettingInstance</span></span>

<span data-ttu-id="d03d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d03d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d03d8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d03d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d03d8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d03d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d03d8-107">Atualize as propriedades de [um objeto deviceManagementAbstractComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d03d8-107">Update the properties of a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d03d8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d03d8-108">Prerequisites</span></span>
<span data-ttu-id="d03d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d03d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d03d8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d03d8-111">Permission type</span></span>|<span data-ttu-id="d03d8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d03d8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d03d8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d03d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d03d8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d03d8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d03d8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d03d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d03d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d03d8-116">Not supported.</span></span>|
|<span data-ttu-id="d03d8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d03d8-117">Application</span></span>|<span data-ttu-id="d03d8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d03d8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d03d8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d03d8-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d03d8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d03d8-120">Request headers</span></span>
|<span data-ttu-id="d03d8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d03d8-121">Header</span></span>|<span data-ttu-id="d03d8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d03d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d03d8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d03d8-123">Authorization</span></span>|<span data-ttu-id="d03d8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d03d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d03d8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d03d8-125">Accept</span></span>|<span data-ttu-id="d03d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d03d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d03d8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d03d8-127">Request body</span></span>
<span data-ttu-id="d03d8-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementAbstractComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d03d8-128">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="d03d8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="d03d8-129">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="d03d8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d03d8-130">Property</span></span>|<span data-ttu-id="d03d8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d03d8-131">Type</span></span>|<span data-ttu-id="d03d8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d03d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d03d8-133">id</span><span class="sxs-lookup"><span data-stu-id="d03d8-133">id</span></span>|<span data-ttu-id="d03d8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d03d8-134">String</span></span>|<span data-ttu-id="d03d8-135">A ID da instância de configuração Herdada [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d03d8-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d03d8-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="d03d8-136">definitionId</span></span>|<span data-ttu-id="d03d8-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d03d8-137">String</span></span>|<span data-ttu-id="d03d8-138">A ID da definição de configuração para esta instância Herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d03d8-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d03d8-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="d03d8-139">valueJson</span></span>|<span data-ttu-id="d03d8-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d03d8-140">String</span></span>|<span data-ttu-id="d03d8-141">Representação JSON do valor Herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d03d8-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d03d8-142">implementationId</span><span class="sxs-lookup"><span data-stu-id="d03d8-142">implementationId</span></span>|<span data-ttu-id="d03d8-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d03d8-143">String</span></span>|<span data-ttu-id="d03d8-144">A ID de definição para a implementação escolhida dessa configuração complexa</span><span class="sxs-lookup"><span data-stu-id="d03d8-144">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="d03d8-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d03d8-145">Response</span></span>
<span data-ttu-id="d03d8-146">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d03d8-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d03d8-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d03d8-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d03d8-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d03d8-148">Request</span></span>
<span data-ttu-id="d03d8-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d03d8-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d03d8-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d03d8-150">Response</span></span>
<span data-ttu-id="d03d8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d03d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




