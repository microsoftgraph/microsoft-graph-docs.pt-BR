---
title: Criar deviceManagementStringSettingInstance
description: Criar um novo objeto deviceManagementStringSettingInstance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c62de0116d64cbad78ef17289f5a062aa42122b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959835"
---
# <a name="create-devicemanagementstringsettinginstance"></a><span data-ttu-id="cb529-103">Criar deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="cb529-103">Create deviceManagementStringSettingInstance</span></span>

> <span data-ttu-id="cb529-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb529-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb529-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb529-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb529-106">Criar um novo objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="cb529-106">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb529-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb529-107">Prerequisites</span></span>
<span data-ttu-id="cb529-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb529-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb529-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb529-110">Permission type</span></span>|<span data-ttu-id="cb529-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cb529-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb529-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb529-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb529-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb529-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cb529-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb529-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb529-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb529-115">Not supported.</span></span>|
|<span data-ttu-id="cb529-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb529-116">Application</span></span>|<span data-ttu-id="cb529-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb529-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb529-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb529-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="cb529-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb529-119">Request headers</span></span>
|<span data-ttu-id="cb529-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb529-120">Header</span></span>|<span data-ttu-id="cb529-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cb529-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb529-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb529-122">Authorization</span></span>|<span data-ttu-id="cb529-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb529-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb529-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cb529-124">Accept</span></span>|<span data-ttu-id="cb529-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb529-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb529-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb529-126">Request body</span></span>
<span data-ttu-id="cb529-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementStringSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="cb529-127">In the request body, supply a JSON representation for the deviceManagementStringSettingInstance object.</span></span>

<span data-ttu-id="cb529-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementStringSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="cb529-128">The following table shows the properties that are required when you create the deviceManagementStringSettingInstance.</span></span>

|<span data-ttu-id="cb529-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb529-129">Property</span></span>|<span data-ttu-id="cb529-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb529-130">Type</span></span>|<span data-ttu-id="cb529-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb529-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb529-132">id</span><span class="sxs-lookup"><span data-stu-id="cb529-132">id</span></span>|<span data-ttu-id="cb529-133">String</span><span class="sxs-lookup"><span data-stu-id="cb529-133">String</span></span>|<span data-ttu-id="cb529-134">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="cb529-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="cb529-135">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="cb529-135">definitionId</span></span>|<span data-ttu-id="cb529-136">String</span><span class="sxs-lookup"><span data-stu-id="cb529-136">String</span></span>|<span data-ttu-id="cb529-137">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="cb529-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="cb529-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="cb529-138">valueJson</span></span>|<span data-ttu-id="cb529-139">String</span><span class="sxs-lookup"><span data-stu-id="cb529-139">String</span></span>|<span data-ttu-id="cb529-140">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="cb529-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="cb529-141">value</span><span class="sxs-lookup"><span data-stu-id="cb529-141">value</span></span>|<span data-ttu-id="cb529-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb529-142">String</span></span>|<span data-ttu-id="cb529-143">O valor da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb529-143">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="cb529-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb529-144">Response</span></span>
<span data-ttu-id="cb529-145">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb529-145">If successful, this method returns a `201 Created` response code and a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb529-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb529-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb529-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb529-147">Request</span></span>
<span data-ttu-id="cb529-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb529-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cb529-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb529-149">Response</span></span>
<span data-ttu-id="cb529-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb529-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





