---
title: Atualizar deviceManagementIntentSettingCategory
description: Atualiza as propriedades de um objeto deviceManagementIntentSettingCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9b878e0bf7ab010d261f7a12ee6c950de8ba9a1d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343458"
---
# <a name="update-devicemanagementintentsettingcategory"></a><span data-ttu-id="a0a03-103">Atualizar deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="a0a03-103">Update deviceManagementIntentSettingCategory</span></span>

> <span data-ttu-id="a0a03-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0a03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0a03-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0a03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0a03-106">Atualiza as propriedades de um objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="a0a03-106">Update the properties of a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0a03-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0a03-107">Prerequisites</span></span>
<span data-ttu-id="a0a03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0a03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0a03-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0a03-110">Permission type</span></span>|<span data-ttu-id="a0a03-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0a03-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0a03-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0a03-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0a03-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0a03-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0a03-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0a03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0a03-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0a03-115">Not supported.</span></span>|
|<span data-ttu-id="a0a03-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0a03-116">Application</span></span>|<span data-ttu-id="a0a03-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0a03-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0a03-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0a03-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="a0a03-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0a03-119">Request headers</span></span>
|<span data-ttu-id="a0a03-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0a03-120">Header</span></span>|<span data-ttu-id="a0a03-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a0a03-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0a03-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0a03-122">Authorization</span></span>|<span data-ttu-id="a0a03-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0a03-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0a03-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0a03-124">Accept</span></span>|<span data-ttu-id="a0a03-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0a03-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0a03-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0a03-126">Request body</span></span>
<span data-ttu-id="a0a03-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="a0a03-127">In the request body, supply a JSON representation for the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

<span data-ttu-id="a0a03-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="a0a03-128">The following table shows the properties that are required when you create the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).</span></span>

|<span data-ttu-id="a0a03-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0a03-129">Property</span></span>|<span data-ttu-id="a0a03-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0a03-130">Type</span></span>|<span data-ttu-id="a0a03-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0a03-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0a03-132">id</span><span class="sxs-lookup"><span data-stu-id="a0a03-132">id</span></span>|<span data-ttu-id="a0a03-133">String</span><span class="sxs-lookup"><span data-stu-id="a0a03-133">String</span></span>|<span data-ttu-id="a0a03-134">A ID de categoria herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="a0a03-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="a0a03-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a0a03-135">displayName</span></span>|<span data-ttu-id="a0a03-136">String</span><span class="sxs-lookup"><span data-stu-id="a0a03-136">String</span></span>|<span data-ttu-id="a0a03-137">O nome da categoria herdado de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="a0a03-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a0a03-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0a03-138">Response</span></span>
<span data-ttu-id="a0a03-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0a03-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0a03-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0a03-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0a03-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0a03-141">Request</span></span>
<span data-ttu-id="a0a03-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0a03-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
Content-type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="a0a03-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0a03-143">Response</span></span>
<span data-ttu-id="a0a03-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0a03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 168

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
  "displayName": "Display Name value"
}
```






