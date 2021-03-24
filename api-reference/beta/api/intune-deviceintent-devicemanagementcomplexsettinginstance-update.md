---
title: Atualizar deviceManagementComplexSettingInstance
description: Atualize as propriedades de um objeto deviceManagementComplexSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80627d958360f18b53a713d3ff94a8699bc50794
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130970"
---
# <a name="update-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="4d7e5-103">Atualizar deviceManagementComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="4d7e5-103">Update deviceManagementComplexSettingInstance</span></span>

<span data-ttu-id="4d7e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d7e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d7e5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d7e5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d7e5-107">Atualize as propriedades de [um objeto deviceManagementComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4d7e5-107">Update the properties of a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d7e5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d7e5-108">Prerequisites</span></span>
<span data-ttu-id="4d7e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d7e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d7e5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d7e5-111">Permission type</span></span>|<span data-ttu-id="4d7e5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d7e5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d7e5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d7e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d7e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d7e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d7e5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d7e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d7e5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-116">Not supported.</span></span>|
|<span data-ttu-id="4d7e5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d7e5-117">Application</span></span>|<span data-ttu-id="4d7e5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d7e5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d7e5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d7e5-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4d7e5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d7e5-120">Request headers</span></span>
|<span data-ttu-id="4d7e5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d7e5-121">Header</span></span>|<span data-ttu-id="4d7e5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4d7e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d7e5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d7e5-123">Authorization</span></span>|<span data-ttu-id="4d7e5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d7e5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4d7e5-125">Accept</span></span>|<span data-ttu-id="4d7e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d7e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d7e5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d7e5-127">Request body</span></span>
<span data-ttu-id="4d7e5-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4d7e5-128">In the request body, supply a JSON representation for the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="4d7e5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="4d7e5-129">The following table shows the properties that are required when you create the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="4d7e5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d7e5-130">Property</span></span>|<span data-ttu-id="4d7e5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d7e5-131">Type</span></span>|<span data-ttu-id="4d7e5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d7e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d7e5-133">id</span><span class="sxs-lookup"><span data-stu-id="4d7e5-133">id</span></span>|<span data-ttu-id="4d7e5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d7e5-134">String</span></span>|<span data-ttu-id="4d7e5-135">A ID da instância de configuração Herdada [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4d7e5-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4d7e5-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="4d7e5-136">definitionId</span></span>|<span data-ttu-id="4d7e5-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d7e5-137">String</span></span>|<span data-ttu-id="4d7e5-138">A ID da definição de configuração para esta instância Herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4d7e5-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4d7e5-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="4d7e5-139">valueJson</span></span>|<span data-ttu-id="4d7e5-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d7e5-140">String</span></span>|<span data-ttu-id="4d7e5-141">Representação JSON do valor Herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4d7e5-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4d7e5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d7e5-142">Response</span></span>
<span data-ttu-id="4d7e5-143">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d7e5-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d7e5-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d7e5-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d7e5-145">Request</span></span>
<span data-ttu-id="4d7e5-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="4d7e5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d7e5-147">Response</span></span>
<span data-ttu-id="4d7e5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d7e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 207

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```




