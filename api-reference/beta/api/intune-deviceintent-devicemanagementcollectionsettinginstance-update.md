---
title: Atualizar deviceManagementCollectionSettingInstance
description: Atualize as propriedades de um objeto deviceManagementCollectionSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 315552c81f6f2d7870574f8900a7d0b60ba00505
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128975"
---
# <a name="update-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="02e92-103">Atualizar deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="02e92-103">Update deviceManagementCollectionSettingInstance</span></span>

<span data-ttu-id="02e92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02e92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02e92-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02e92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02e92-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02e92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02e92-107">Atualize as propriedades de [um objeto deviceManagementCollectionSettingInstance.](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="02e92-107">Update the properties of a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02e92-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02e92-108">Prerequisites</span></span>
<span data-ttu-id="02e92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02e92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02e92-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02e92-111">Permission type</span></span>|<span data-ttu-id="02e92-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02e92-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02e92-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02e92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02e92-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02e92-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02e92-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02e92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02e92-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02e92-116">Not supported.</span></span>|
|<span data-ttu-id="02e92-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02e92-117">Application</span></span>|<span data-ttu-id="02e92-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02e92-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02e92-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02e92-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="02e92-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02e92-120">Request headers</span></span>
|<span data-ttu-id="02e92-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02e92-121">Header</span></span>|<span data-ttu-id="02e92-122">Valor</span><span class="sxs-lookup"><span data-stu-id="02e92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02e92-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02e92-123">Authorization</span></span>|<span data-ttu-id="02e92-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02e92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02e92-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02e92-125">Accept</span></span>|<span data-ttu-id="02e92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02e92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02e92-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02e92-127">Request body</span></span>
<span data-ttu-id="02e92-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementCollectionSettingInstance.](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="02e92-128">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

<span data-ttu-id="02e92-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="02e92-129">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span></span>

|<span data-ttu-id="02e92-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02e92-130">Property</span></span>|<span data-ttu-id="02e92-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02e92-131">Type</span></span>|<span data-ttu-id="02e92-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02e92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02e92-133">id</span><span class="sxs-lookup"><span data-stu-id="02e92-133">id</span></span>|<span data-ttu-id="02e92-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02e92-134">String</span></span>|<span data-ttu-id="02e92-135">A ID da instância de configuração Herdada [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="02e92-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="02e92-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="02e92-136">definitionId</span></span>|<span data-ttu-id="02e92-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02e92-137">String</span></span>|<span data-ttu-id="02e92-138">A ID da definição de configuração para esta instância Herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="02e92-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="02e92-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="02e92-139">valueJson</span></span>|<span data-ttu-id="02e92-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02e92-140">String</span></span>|<span data-ttu-id="02e92-141">Representação JSON do valor Herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="02e92-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="02e92-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="02e92-142">Response</span></span>
<span data-ttu-id="02e92-143">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02e92-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02e92-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02e92-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="02e92-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02e92-145">Request</span></span>
<span data-ttu-id="02e92-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02e92-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="02e92-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="02e92-147">Response</span></span>
<span data-ttu-id="02e92-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02e92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




