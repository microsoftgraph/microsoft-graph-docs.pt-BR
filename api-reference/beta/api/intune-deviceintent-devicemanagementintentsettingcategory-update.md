---
title: Atualizar deviceManagementIntentSettingCategory
description: Atualiza as propriedades de um objeto deviceManagementIntentSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f443e21653aa53a86c5080d5636912c163a98798
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306300"
---
# <a name="update-devicemanagementintentsettingcategory"></a><span data-ttu-id="646ec-103">Atualizar deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="646ec-103">Update deviceManagementIntentSettingCategory</span></span>

<span data-ttu-id="646ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="646ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="646ec-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="646ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="646ec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="646ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="646ec-107">Atualiza as propriedades de um objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="646ec-107">Update the properties of a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="646ec-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="646ec-108">Prerequisites</span></span>
<span data-ttu-id="646ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="646ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="646ec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="646ec-111">Permission type</span></span>|<span data-ttu-id="646ec-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="646ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="646ec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="646ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="646ec-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="646ec-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="646ec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="646ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="646ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="646ec-116">Not supported.</span></span>|
|<span data-ttu-id="646ec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="646ec-117">Application</span></span>|<span data-ttu-id="646ec-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="646ec-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="646ec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="646ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="646ec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="646ec-120">Request headers</span></span>
|<span data-ttu-id="646ec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="646ec-121">Header</span></span>|<span data-ttu-id="646ec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="646ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="646ec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="646ec-123">Authorization</span></span>|<span data-ttu-id="646ec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="646ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="646ec-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="646ec-125">Accept</span></span>|<span data-ttu-id="646ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="646ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="646ec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="646ec-127">Request body</span></span>
<span data-ttu-id="646ec-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="646ec-128">In the request body, supply a JSON representation for the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

<span data-ttu-id="646ec-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="646ec-129">The following table shows the properties that are required when you create the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).</span></span>

|<span data-ttu-id="646ec-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="646ec-130">Property</span></span>|<span data-ttu-id="646ec-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="646ec-131">Type</span></span>|<span data-ttu-id="646ec-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="646ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="646ec-133">id</span><span class="sxs-lookup"><span data-stu-id="646ec-133">id</span></span>|<span data-ttu-id="646ec-134">String</span><span class="sxs-lookup"><span data-stu-id="646ec-134">String</span></span>|<span data-ttu-id="646ec-135">A ID de categoria herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="646ec-135">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="646ec-136">displayName</span><span class="sxs-lookup"><span data-stu-id="646ec-136">displayName</span></span>|<span data-ttu-id="646ec-137">String</span><span class="sxs-lookup"><span data-stu-id="646ec-137">String</span></span>|<span data-ttu-id="646ec-138">O nome da categoria herdado de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="646ec-138">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="646ec-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="646ec-139">hasRequiredSetting</span></span>|<span data-ttu-id="646ec-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="646ec-140">Boolean</span></span>|<span data-ttu-id="646ec-141">A categoria contém a configuração necessária de nível superior herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="646ec-141">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="646ec-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="646ec-142">Response</span></span>
<span data-ttu-id="646ec-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="646ec-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="646ec-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="646ec-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="646ec-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="646ec-145">Request</span></span>
<span data-ttu-id="646ec-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="646ec-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
Content-type: application/json
Content-length: 150

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="646ec-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="646ec-147">Response</span></span>
<span data-ttu-id="646ec-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="646ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 199

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




