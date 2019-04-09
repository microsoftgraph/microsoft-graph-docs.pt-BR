---
title: Criar deviceManagementStringSettingInstance
description: Criar um novo objeto deviceManagementStringSettingInstance.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 615b8d7a6cdae5b8f1d881181b80815f94cc508a
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522752"
---
# <a name="create-devicemanagementstringsettinginstance"></a><span data-ttu-id="c0833-103">Criar deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="c0833-103">Create deviceManagementStringSettingInstance</span></span>

> <span data-ttu-id="c0833-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0833-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0833-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0833-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0833-106">Criar um novo objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="c0833-106">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0833-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0833-107">Prerequisites</span></span>
<span data-ttu-id="c0833-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0833-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0833-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0833-110">Permission type</span></span>|<span data-ttu-id="c0833-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0833-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0833-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0833-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0833-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0833-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0833-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0833-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0833-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0833-115">Not supported.</span></span>|
|<span data-ttu-id="c0833-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0833-116">Application</span></span>|<span data-ttu-id="c0833-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0833-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0833-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0833-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c0833-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0833-119">Request headers</span></span>
|<span data-ttu-id="c0833-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0833-120">Header</span></span>|<span data-ttu-id="c0833-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c0833-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0833-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0833-122">Authorization</span></span>|<span data-ttu-id="c0833-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0833-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0833-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0833-124">Accept</span></span>|<span data-ttu-id="c0833-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0833-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0833-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0833-126">Request body</span></span>
<span data-ttu-id="c0833-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementStringSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="c0833-127">In the request body, supply a JSON representation for the deviceManagementStringSettingInstance object.</span></span>

<span data-ttu-id="c0833-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementStringSettingInstance.</span><span class="sxs-lookup"><span data-stu-id="c0833-128">The following table shows the properties that are required when you create the deviceManagementStringSettingInstance.</span></span>

|<span data-ttu-id="c0833-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0833-129">Property</span></span>|<span data-ttu-id="c0833-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0833-130">Type</span></span>|<span data-ttu-id="c0833-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0833-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0833-132">id</span><span class="sxs-lookup"><span data-stu-id="c0833-132">id</span></span>|<span data-ttu-id="c0833-133">String</span><span class="sxs-lookup"><span data-stu-id="c0833-133">String</span></span>|<span data-ttu-id="c0833-134">A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="c0833-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="c0833-135">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="c0833-135">definitionId</span></span>|<span data-ttu-id="c0833-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="c0833-136">String</span></span>|<span data-ttu-id="c0833-137">A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="c0833-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="c0833-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="c0833-138">valueJson</span></span>|<span data-ttu-id="c0833-139">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="c0833-139">String</span></span>|<span data-ttu-id="c0833-140">Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="c0833-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="c0833-141">value</span><span class="sxs-lookup"><span data-stu-id="c0833-141">value</span></span>|<span data-ttu-id="c0833-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0833-142">String</span></span>|<span data-ttu-id="c0833-143">O valor da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0833-143">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="c0833-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0833-144">Response</span></span>
<span data-ttu-id="c0833-145">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0833-145">If successful, this method returns a `201 Created` response code and a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0833-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0833-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0833-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0833-147">Request</span></span>
<span data-ttu-id="c0833-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0833-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c0833-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0833-149">Response</span></span>
<span data-ttu-id="c0833-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0833-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







