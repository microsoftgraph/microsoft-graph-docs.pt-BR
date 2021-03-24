---
title: Atualizar deviceManagementIntegerSettingInstance
description: Atualize as propriedades de um objeto deviceManagementIntegerSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b90a762699336fe0874790d5e0553c077b80095
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132090"
---
# <a name="update-devicemanagementintegersettinginstance"></a><span data-ttu-id="983ab-103">Atualizar deviceManagementIntegerSettingInstance</span><span class="sxs-lookup"><span data-stu-id="983ab-103">Update deviceManagementIntegerSettingInstance</span></span>

<span data-ttu-id="983ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="983ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="983ab-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="983ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="983ab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="983ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="983ab-107">Atualize as propriedades de [um objeto deviceManagementIntegerSettingInstance.](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="983ab-107">Update the properties of a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="983ab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="983ab-108">Prerequisites</span></span>
<span data-ttu-id="983ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="983ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="983ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="983ab-111">Permission type</span></span>|<span data-ttu-id="983ab-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="983ab-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="983ab-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="983ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="983ab-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="983ab-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="983ab-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="983ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="983ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="983ab-116">Not supported.</span></span>|
|<span data-ttu-id="983ab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="983ab-117">Application</span></span>|<span data-ttu-id="983ab-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="983ab-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="983ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="983ab-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="983ab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="983ab-120">Request headers</span></span>
|<span data-ttu-id="983ab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="983ab-121">Header</span></span>|<span data-ttu-id="983ab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="983ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="983ab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="983ab-123">Authorization</span></span>|<span data-ttu-id="983ab-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="983ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="983ab-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="983ab-125">Accept</span></span>|<span data-ttu-id="983ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="983ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="983ab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="983ab-127">Request body</span></span>
<span data-ttu-id="983ab-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementIntegerSettingInstance.](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="983ab-128">In the request body, supply a JSON representation for the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

<span data-ttu-id="983ab-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="983ab-129">The following table shows the properties that are required when you create the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span></span>

|<span data-ttu-id="983ab-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="983ab-130">Property</span></span>|<span data-ttu-id="983ab-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="983ab-131">Type</span></span>|<span data-ttu-id="983ab-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="983ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="983ab-133">id</span><span class="sxs-lookup"><span data-stu-id="983ab-133">id</span></span>|<span data-ttu-id="983ab-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="983ab-134">String</span></span>|<span data-ttu-id="983ab-135">A ID da instância de configuração Herdada [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="983ab-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="983ab-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="983ab-136">definitionId</span></span>|<span data-ttu-id="983ab-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="983ab-137">String</span></span>|<span data-ttu-id="983ab-138">A ID da definição de configuração para esta instância Herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="983ab-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="983ab-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="983ab-139">valueJson</span></span>|<span data-ttu-id="983ab-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="983ab-140">String</span></span>|<span data-ttu-id="983ab-141">Representação JSON do valor Herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="983ab-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="983ab-142">valor</span><span class="sxs-lookup"><span data-stu-id="983ab-142">value</span></span>|<span data-ttu-id="983ab-143">Int32</span><span class="sxs-lookup"><span data-stu-id="983ab-143">Int32</span></span>|<span data-ttu-id="983ab-144">O valor inteiro</span><span class="sxs-lookup"><span data-stu-id="983ab-144">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="983ab-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="983ab-145">Response</span></span>
<span data-ttu-id="983ab-146">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="983ab-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="983ab-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="983ab-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="983ab-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="983ab-148">Request</span></span>
<span data-ttu-id="983ab-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="983ab-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="983ab-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="983ab-150">Response</span></span>
<span data-ttu-id="983ab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="983ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "id": "60468ce7-8ce7-6046-e78c-4660e78c4660",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```




