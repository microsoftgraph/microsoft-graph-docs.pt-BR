---
title: Criar deviceManagementIntentSettingCategory
description: Criar um novo objeto deviceManagementIntentSettingCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c92ab47984984bc97e37ab071798ba345a0c963c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470872"
---
# <a name="create-devicemanagementintentsettingcategory"></a><span data-ttu-id="f1024-103">Criar deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="f1024-103">Create deviceManagementIntentSettingCategory</span></span>

<span data-ttu-id="f1024-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f1024-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1024-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1024-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1024-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1024-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1024-107">Criar um novo objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="f1024-107">Create a new [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1024-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1024-108">Prerequisites</span></span>
<span data-ttu-id="f1024-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1024-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1024-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1024-111">Permission type</span></span>|<span data-ttu-id="f1024-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1024-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1024-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1024-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1024-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1024-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1024-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1024-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1024-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1024-116">Not supported.</span></span>|
|<span data-ttu-id="f1024-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1024-117">Application</span></span>|<span data-ttu-id="f1024-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1024-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1024-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1024-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="f1024-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1024-120">Request headers</span></span>
|<span data-ttu-id="f1024-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1024-121">Header</span></span>|<span data-ttu-id="f1024-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f1024-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1024-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1024-123">Authorization</span></span>|<span data-ttu-id="f1024-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1024-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1024-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1024-125">Accept</span></span>|<span data-ttu-id="f1024-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1024-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1024-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1024-127">Request body</span></span>
<span data-ttu-id="f1024-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntentSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="f1024-128">In the request body, supply a JSON representation for the deviceManagementIntentSettingCategory object.</span></span>

<span data-ttu-id="f1024-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntentSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="f1024-129">The following table shows the properties that are required when you create the deviceManagementIntentSettingCategory.</span></span>

|<span data-ttu-id="f1024-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1024-130">Property</span></span>|<span data-ttu-id="f1024-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1024-131">Type</span></span>|<span data-ttu-id="f1024-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1024-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1024-133">id</span><span class="sxs-lookup"><span data-stu-id="f1024-133">id</span></span>|<span data-ttu-id="f1024-134">String</span><span class="sxs-lookup"><span data-stu-id="f1024-134">String</span></span>|<span data-ttu-id="f1024-135">A ID de categoria herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="f1024-135">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="f1024-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f1024-136">displayName</span></span>|<span data-ttu-id="f1024-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1024-137">String</span></span>|<span data-ttu-id="f1024-138">O nome da categoria herdado de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="f1024-138">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="f1024-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="f1024-139">hasRequiredSetting</span></span>|<span data-ttu-id="f1024-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1024-140">Boolean</span></span>|<span data-ttu-id="f1024-141">A categoria contém a configuração necessária de nível superior herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="f1024-141">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f1024-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1024-142">Response</span></span>
<span data-ttu-id="f1024-143">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1024-143">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1024-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1024-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1024-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1024-145">Request</span></span>
<span data-ttu-id="f1024-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1024-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1024-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1024-147">Response</span></span>
<span data-ttu-id="f1024-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1024-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





