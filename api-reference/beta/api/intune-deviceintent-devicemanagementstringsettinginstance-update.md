---
title: Atualizar deviceManagementStringSettingInstance
description: Atualize as propriedades de um objeto deviceManagementStringSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9094bb663e3080177da82589b165ba539b360a14
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150735"
---
# <a name="update-devicemanagementstringsettinginstance"></a><span data-ttu-id="dc774-103">Atualizar deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="dc774-103">Update deviceManagementStringSettingInstance</span></span>

<span data-ttu-id="dc774-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc774-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc774-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc774-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc774-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc774-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc774-107">Atualize as propriedades de [um objeto deviceManagementStringSettingInstance.](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dc774-107">Update the properties of a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc774-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc774-108">Prerequisites</span></span>
<span data-ttu-id="dc774-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc774-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc774-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc774-111">Permission type</span></span>|<span data-ttu-id="dc774-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc774-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc774-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc774-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc774-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc774-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc774-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc774-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc774-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc774-116">Not supported.</span></span>|
|<span data-ttu-id="dc774-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc774-117">Application</span></span>|<span data-ttu-id="dc774-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc774-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc774-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc774-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="dc774-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc774-120">Request headers</span></span>
|<span data-ttu-id="dc774-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc774-121">Header</span></span>|<span data-ttu-id="dc774-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dc774-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc774-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc774-123">Authorization</span></span>|<span data-ttu-id="dc774-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc774-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc774-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc774-125">Accept</span></span>|<span data-ttu-id="dc774-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc774-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc774-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc774-127">Request body</span></span>
<span data-ttu-id="dc774-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementStringSettingInstance.](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dc774-128">In the request body, supply a JSON representation for the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

<span data-ttu-id="dc774-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="dc774-129">The following table shows the properties that are required when you create the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span></span>

|<span data-ttu-id="dc774-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc774-130">Property</span></span>|<span data-ttu-id="dc774-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc774-131">Type</span></span>|<span data-ttu-id="dc774-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc774-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc774-133">id</span><span class="sxs-lookup"><span data-stu-id="dc774-133">id</span></span>|<span data-ttu-id="dc774-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc774-134">String</span></span>|<span data-ttu-id="dc774-135">A ID da instância de configuração Herdada [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dc774-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="dc774-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="dc774-136">definitionId</span></span>|<span data-ttu-id="dc774-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc774-137">String</span></span>|<span data-ttu-id="dc774-138">A ID da definição de configuração para esta instância Herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dc774-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="dc774-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="dc774-139">valueJson</span></span>|<span data-ttu-id="dc774-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc774-140">String</span></span>|<span data-ttu-id="dc774-141">Representação JSON do valor Herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dc774-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="dc774-142">value</span><span class="sxs-lookup"><span data-stu-id="dc774-142">value</span></span>|<span data-ttu-id="dc774-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc774-143">String</span></span>|<span data-ttu-id="dc774-144">O valor da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc774-144">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="dc774-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc774-145">Response</span></span>
<span data-ttu-id="dc774-146">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc774-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc774-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc774-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc774-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc774-148">Request</span></span>
<span data-ttu-id="dc774-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc774-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="dc774-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc774-150">Response</span></span>
<span data-ttu-id="dc774-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc774-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




