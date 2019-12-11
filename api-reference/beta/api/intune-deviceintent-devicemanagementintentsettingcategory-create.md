---
title: Criar deviceManagementIntentSettingCategory
description: Criar um novo objeto deviceManagementIntentSettingCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b361d9d37cdde99e1a96918e53b21ee19d60a279
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945708"
---
# <a name="create-devicemanagementintentsettingcategory"></a><span data-ttu-id="8bc69-103">Criar deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="8bc69-103">Create deviceManagementIntentSettingCategory</span></span>

> <span data-ttu-id="8bc69-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8bc69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bc69-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8bc69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bc69-106">Criar um novo objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="8bc69-106">Create a new [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bc69-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8bc69-107">Prerequisites</span></span>
<span data-ttu-id="8bc69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bc69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bc69-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bc69-110">Permission type</span></span>|<span data-ttu-id="8bc69-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8bc69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bc69-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bc69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8bc69-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bc69-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8bc69-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bc69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bc69-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bc69-115">Not supported.</span></span>|
|<span data-ttu-id="8bc69-116">Application</span><span class="sxs-lookup"><span data-stu-id="8bc69-116">Application</span></span>|<span data-ttu-id="8bc69-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bc69-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bc69-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bc69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="8bc69-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bc69-119">Request headers</span></span>
|<span data-ttu-id="8bc69-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8bc69-120">Header</span></span>|<span data-ttu-id="8bc69-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8bc69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bc69-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bc69-122">Authorization</span></span>|<span data-ttu-id="8bc69-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bc69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bc69-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8bc69-124">Accept</span></span>|<span data-ttu-id="8bc69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8bc69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bc69-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bc69-126">Request body</span></span>
<span data-ttu-id="8bc69-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntentSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="8bc69-127">In the request body, supply a JSON representation for the deviceManagementIntentSettingCategory object.</span></span>

<span data-ttu-id="8bc69-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntentSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="8bc69-128">The following table shows the properties that are required when you create the deviceManagementIntentSettingCategory.</span></span>

|<span data-ttu-id="8bc69-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8bc69-129">Property</span></span>|<span data-ttu-id="8bc69-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bc69-130">Type</span></span>|<span data-ttu-id="8bc69-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bc69-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bc69-132">id</span><span class="sxs-lookup"><span data-stu-id="8bc69-132">id</span></span>|<span data-ttu-id="8bc69-133">String</span><span class="sxs-lookup"><span data-stu-id="8bc69-133">String</span></span>|<span data-ttu-id="8bc69-134">A ID de categoria herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="8bc69-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="8bc69-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8bc69-135">displayName</span></span>|<span data-ttu-id="8bc69-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bc69-136">String</span></span>|<span data-ttu-id="8bc69-137">O nome da categoria herdado de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="8bc69-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8bc69-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bc69-138">Response</span></span>
<span data-ttu-id="8bc69-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bc69-139">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bc69-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bc69-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bc69-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bc69-141">Request</span></span>
<span data-ttu-id="8bc69-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bc69-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories
Content-type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="8bc69-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bc69-143">Response</span></span>
<span data-ttu-id="8bc69-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bc69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 168

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
  "displayName": "Display Name value"
}
```





