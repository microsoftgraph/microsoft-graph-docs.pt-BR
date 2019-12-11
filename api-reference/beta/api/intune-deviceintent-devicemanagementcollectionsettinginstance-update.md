---
title: Atualizar deviceManagementCollectionSettingInstance
description: Atualiza as propriedades de um objeto deviceManagementCollectionSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1e7b6b198ea1d17ffed1e9d662c9e17d97c7828a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946081"
---
# <a name="update-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="9acdc-103">Atualizar deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="9acdc-103">Update deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="9acdc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9acdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9acdc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9acdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9acdc-106">Atualiza as propriedades de um objeto [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="9acdc-106">Update the properties of a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9acdc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9acdc-107">Prerequisites</span></span>
<span data-ttu-id="9acdc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9acdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9acdc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9acdc-110">Permission type</span></span>|<span data-ttu-id="9acdc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9acdc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9acdc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9acdc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9acdc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9acdc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9acdc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9acdc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9acdc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9acdc-115">Not supported.</span></span>|
|<span data-ttu-id="9acdc-116">Application</span><span class="sxs-lookup"><span data-stu-id="9acdc-116">Application</span></span>|<span data-ttu-id="9acdc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9acdc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9acdc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9acdc-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9acdc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9acdc-119">Request headers</span></span>
|<span data-ttu-id="9acdc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9acdc-120">Header</span></span>|<span data-ttu-id="9acdc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9acdc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9acdc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9acdc-122">Authorization</span></span>|<span data-ttu-id="9acdc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9acdc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9acdc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9acdc-124">Accept</span></span>|<span data-ttu-id="9acdc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9acdc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9acdc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9acdc-126">Request body</span></span>
<span data-ttu-id="9acdc-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="9acdc-127">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

<span data-ttu-id="9acdc-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="9acdc-128">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span></span>

|<span data-ttu-id="9acdc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9acdc-129">Property</span></span>|<span data-ttu-id="9acdc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9acdc-130">Type</span></span>|<span data-ttu-id="9acdc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9acdc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9acdc-132">id</span><span class="sxs-lookup"><span data-stu-id="9acdc-132">id</span></span>|<span data-ttu-id="9acdc-133">String</span><span class="sxs-lookup"><span data-stu-id="9acdc-133">String</span></span>|<span data-ttu-id="9acdc-134">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="9acdc-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9acdc-135">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="9acdc-135">definitionId</span></span>|<span data-ttu-id="9acdc-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="9acdc-136">String</span></span>|<span data-ttu-id="9acdc-137">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="9acdc-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9acdc-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="9acdc-138">valueJson</span></span>|<span data-ttu-id="9acdc-139">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="9acdc-139">String</span></span>|<span data-ttu-id="9acdc-140">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="9acdc-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9acdc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9acdc-141">Response</span></span>
<span data-ttu-id="9acdc-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9acdc-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9acdc-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9acdc-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="9acdc-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9acdc-144">Request</span></span>
<span data-ttu-id="9acdc-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9acdc-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="9acdc-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9acdc-146">Response</span></span>
<span data-ttu-id="9acdc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9acdc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```





