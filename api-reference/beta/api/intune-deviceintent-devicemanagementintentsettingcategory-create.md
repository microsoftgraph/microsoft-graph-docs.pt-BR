---
title: Criar deviceManagementIntentSettingCategory
description: Crie um novo objeto deviceManagementIntentSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a56f0ef9859038fb43cdadab4548a43245f64b0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130956"
---
# <a name="create-devicemanagementintentsettingcategory"></a><span data-ttu-id="4b09d-103">Criar deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="4b09d-103">Create deviceManagementIntentSettingCategory</span></span>

<span data-ttu-id="4b09d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b09d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b09d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b09d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b09d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b09d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b09d-107">Crie um novo [objeto deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="4b09d-107">Create a new [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b09d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b09d-108">Prerequisites</span></span>
<span data-ttu-id="4b09d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b09d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b09d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b09d-111">Permission type</span></span>|<span data-ttu-id="4b09d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b09d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b09d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b09d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b09d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b09d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b09d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b09d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b09d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b09d-116">Not supported.</span></span>|
|<span data-ttu-id="4b09d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b09d-117">Application</span></span>|<span data-ttu-id="4b09d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b09d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b09d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b09d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="4b09d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b09d-120">Request headers</span></span>
|<span data-ttu-id="4b09d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b09d-121">Header</span></span>|<span data-ttu-id="4b09d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4b09d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b09d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b09d-123">Authorization</span></span>|<span data-ttu-id="4b09d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b09d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b09d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b09d-125">Accept</span></span>|<span data-ttu-id="4b09d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b09d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b09d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b09d-127">Request body</span></span>
<span data-ttu-id="4b09d-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementIntentSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="4b09d-128">In the request body, supply a JSON representation for the deviceManagementIntentSettingCategory object.</span></span>

<span data-ttu-id="4b09d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntentSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="4b09d-129">The following table shows the properties that are required when you create the deviceManagementIntentSettingCategory.</span></span>

|<span data-ttu-id="4b09d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b09d-130">Property</span></span>|<span data-ttu-id="4b09d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b09d-131">Type</span></span>|<span data-ttu-id="4b09d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b09d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b09d-133">id</span><span class="sxs-lookup"><span data-stu-id="4b09d-133">id</span></span>|<span data-ttu-id="4b09d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b09d-134">String</span></span>|<span data-ttu-id="4b09d-135">A ID da categoria Herdada [de deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="4b09d-135">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="4b09d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4b09d-136">displayName</span></span>|<span data-ttu-id="4b09d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b09d-137">String</span></span>|<span data-ttu-id="4b09d-138">O nome da categoria Herdado [de deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="4b09d-138">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="4b09d-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="4b09d-139">hasRequiredSetting</span></span>|<span data-ttu-id="4b09d-140">Booleano</span><span class="sxs-lookup"><span data-stu-id="4b09d-140">Boolean</span></span>|<span data-ttu-id="4b09d-141">A categoria contém a configuração de nível superior necessária Herdada [de deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="4b09d-141">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4b09d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b09d-142">Response</span></span>
<span data-ttu-id="4b09d-143">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b09d-143">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b09d-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b09d-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b09d-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b09d-145">Request</span></span>
<span data-ttu-id="4b09d-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b09d-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories
Content-type: application/json
Content-length: 150

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="4b09d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b09d-147">Response</span></span>
<span data-ttu-id="4b09d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b09d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 199

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




