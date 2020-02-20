---
title: Atualizar deviceManagementIntentSettingCategory
description: Atualiza as propriedades de um objeto deviceManagementIntentSettingCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 19a9aa8c06428eae5487c896189380047abf238d
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162411"
---
# <a name="update-devicemanagementintentsettingcategory"></a><span data-ttu-id="861be-103">Atualizar deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="861be-103">Update deviceManagementIntentSettingCategory</span></span>

> <span data-ttu-id="861be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="861be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="861be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="861be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="861be-106">Atualiza as propriedades de um objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="861be-106">Update the properties of a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="861be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="861be-107">Prerequisites</span></span>
<span data-ttu-id="861be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="861be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="861be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="861be-110">Permission type</span></span>|<span data-ttu-id="861be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="861be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="861be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="861be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="861be-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861be-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="861be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="861be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="861be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="861be-115">Not supported.</span></span>|
|<span data-ttu-id="861be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="861be-116">Application</span></span>|<span data-ttu-id="861be-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861be-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="861be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="861be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="861be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="861be-119">Request headers</span></span>
|<span data-ttu-id="861be-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="861be-120">Header</span></span>|<span data-ttu-id="861be-121">Valor</span><span class="sxs-lookup"><span data-stu-id="861be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="861be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="861be-122">Authorization</span></span>|<span data-ttu-id="861be-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="861be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="861be-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="861be-124">Accept</span></span>|<span data-ttu-id="861be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="861be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="861be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="861be-126">Request body</span></span>
<span data-ttu-id="861be-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="861be-127">In the request body, supply a JSON representation for the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

<span data-ttu-id="861be-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="861be-128">The following table shows the properties that are required when you create the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).</span></span>

|<span data-ttu-id="861be-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="861be-129">Property</span></span>|<span data-ttu-id="861be-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="861be-130">Type</span></span>|<span data-ttu-id="861be-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="861be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="861be-132">id</span><span class="sxs-lookup"><span data-stu-id="861be-132">id</span></span>|<span data-ttu-id="861be-133">String</span><span class="sxs-lookup"><span data-stu-id="861be-133">String</span></span>|<span data-ttu-id="861be-134">A ID de categoria herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="861be-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="861be-135">displayName</span><span class="sxs-lookup"><span data-stu-id="861be-135">displayName</span></span>|<span data-ttu-id="861be-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="861be-136">String</span></span>|<span data-ttu-id="861be-137">O nome da categoria herdado de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="861be-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="861be-138">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="861be-138">hasRequiredSetting</span></span>|<span data-ttu-id="861be-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="861be-139">Boolean</span></span>|<span data-ttu-id="861be-140">A categoria contém a configuração necessária de nível superior herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="861be-140">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="861be-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="861be-141">Response</span></span>
<span data-ttu-id="861be-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="861be-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="861be-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="861be-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="861be-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="861be-144">Request</span></span>
<span data-ttu-id="861be-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="861be-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="861be-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="861be-146">Response</span></span>
<span data-ttu-id="861be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="861be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





