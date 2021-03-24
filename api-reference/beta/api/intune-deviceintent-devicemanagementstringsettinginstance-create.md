---
title: Criar deviceManagementStringSettingInstance
description: Crie um novo objeto deviceManagementStringSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ecde3da02de6f209d0b950517456e3c368d4175
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128709"
---
# <a name="create-devicemanagementstringsettinginstance"></a><span data-ttu-id="94f98-103">Criar deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="94f98-103">Create deviceManagementStringSettingInstance</span></span>

<span data-ttu-id="94f98-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94f98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94f98-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94f98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94f98-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94f98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94f98-107">Crie um novo [objeto deviceManagementStringSettingInstance.](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="94f98-107">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94f98-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94f98-108">Prerequisites</span></span>
<span data-ttu-id="94f98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94f98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94f98-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94f98-111">Permission type</span></span>|<span data-ttu-id="94f98-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94f98-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94f98-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94f98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94f98-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f98-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="94f98-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94f98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94f98-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94f98-116">Not supported.</span></span>|
|<span data-ttu-id="94f98-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94f98-117">Application</span></span>|<span data-ttu-id="94f98-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f98-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94f98-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94f98-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="94f98-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94f98-120">Request headers</span></span>
|<span data-ttu-id="94f98-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94f98-121">Header</span></span>|<span data-ttu-id="94f98-122">Valor</span><span class="sxs-lookup"><span data-stu-id="94f98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94f98-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="94f98-123">Authorization</span></span>|<span data-ttu-id="94f98-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94f98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94f98-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94f98-125">Accept</span></span>|<span data-ttu-id="94f98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94f98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94f98-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94f98-127">Request body</span></span>
<span data-ttu-id="94f98-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementStringSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="94f98-128">In the request body, supply a JSON representation for the deviceManagementStringSettingInstance object.</span></span>

<span data-ttu-id="94f98-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementStringSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="94f98-129">The following table shows the properties that are required when you create the deviceManagementStringSettingInstance.</span></span>

|<span data-ttu-id="94f98-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94f98-130">Property</span></span>|<span data-ttu-id="94f98-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="94f98-131">Type</span></span>|<span data-ttu-id="94f98-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="94f98-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94f98-133">id</span><span class="sxs-lookup"><span data-stu-id="94f98-133">id</span></span>|<span data-ttu-id="94f98-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94f98-134">String</span></span>|<span data-ttu-id="94f98-135">A ID da instância de configuração Herdada [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="94f98-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="94f98-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="94f98-136">definitionId</span></span>|<span data-ttu-id="94f98-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94f98-137">String</span></span>|<span data-ttu-id="94f98-138">A ID da definição de configuração para esta instância Herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="94f98-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="94f98-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="94f98-139">valueJson</span></span>|<span data-ttu-id="94f98-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94f98-140">String</span></span>|<span data-ttu-id="94f98-141">Representação JSON do valor Herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="94f98-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="94f98-142">value</span><span class="sxs-lookup"><span data-stu-id="94f98-142">value</span></span>|<span data-ttu-id="94f98-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94f98-143">String</span></span>|<span data-ttu-id="94f98-144">O valor da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94f98-144">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="94f98-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="94f98-145">Response</span></span>
<span data-ttu-id="94f98-146">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94f98-146">If successful, this method returns a `201 Created` response code and a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94f98-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94f98-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="94f98-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94f98-148">Request</span></span>
<span data-ttu-id="94f98-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94f98-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="94f98-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="94f98-150">Response</span></span>
<span data-ttu-id="94f98-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94f98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




