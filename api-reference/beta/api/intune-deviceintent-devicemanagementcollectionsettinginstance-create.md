---
title: Criar deviceManagementCollectionSettingInstance
description: Crie um novo objeto deviceManagementCollectionSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cdf43022cb12c212daf408911479d6cdb8bd55a3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129024"
---
# <a name="create-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="581e1-103">Criar deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="581e1-103">Create deviceManagementCollectionSettingInstance</span></span>

<span data-ttu-id="581e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="581e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="581e1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="581e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="581e1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="581e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="581e1-107">Crie um novo [objeto deviceManagementCollectionSettingInstance.](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="581e1-107">Create a new [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="581e1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="581e1-108">Prerequisites</span></span>
<span data-ttu-id="581e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="581e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="581e1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="581e1-111">Permission type</span></span>|<span data-ttu-id="581e1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="581e1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="581e1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="581e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="581e1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="581e1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="581e1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="581e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="581e1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="581e1-116">Not supported.</span></span>|
|<span data-ttu-id="581e1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="581e1-117">Application</span></span>|<span data-ttu-id="581e1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="581e1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="581e1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="581e1-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="581e1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="581e1-120">Request headers</span></span>
|<span data-ttu-id="581e1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="581e1-121">Header</span></span>|<span data-ttu-id="581e1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="581e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="581e1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="581e1-123">Authorization</span></span>|<span data-ttu-id="581e1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="581e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="581e1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="581e1-125">Accept</span></span>|<span data-ttu-id="581e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="581e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="581e1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="581e1-127">Request body</span></span>
<span data-ttu-id="581e1-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementCollectionSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="581e1-128">In the request body, supply a JSON representation for the deviceManagementCollectionSettingInstance object.</span></span>

<span data-ttu-id="581e1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementCollectionSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="581e1-129">The following table shows the properties that are required when you create the deviceManagementCollectionSettingInstance.</span></span>

|<span data-ttu-id="581e1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="581e1-130">Property</span></span>|<span data-ttu-id="581e1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="581e1-131">Type</span></span>|<span data-ttu-id="581e1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="581e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="581e1-133">id</span><span class="sxs-lookup"><span data-stu-id="581e1-133">id</span></span>|<span data-ttu-id="581e1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="581e1-134">String</span></span>|<span data-ttu-id="581e1-135">A ID da instância de configuração Herdada [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="581e1-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="581e1-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="581e1-136">definitionId</span></span>|<span data-ttu-id="581e1-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="581e1-137">String</span></span>|<span data-ttu-id="581e1-138">A ID da definição de configuração para esta instância Herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="581e1-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="581e1-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="581e1-139">valueJson</span></span>|<span data-ttu-id="581e1-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="581e1-140">String</span></span>|<span data-ttu-id="581e1-141">Representação JSON do valor Herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="581e1-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="581e1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="581e1-142">Response</span></span>
<span data-ttu-id="581e1-143">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="581e1-143">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="581e1-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="581e1-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="581e1-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="581e1-145">Request</span></span>
<span data-ttu-id="581e1-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="581e1-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="581e1-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="581e1-147">Response</span></span>
<span data-ttu-id="581e1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="581e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```




