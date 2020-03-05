---
title: Atualizar deviceManagementTemplateSettingCategory
description: Atualiza as propriedades de um objeto deviceManagementTemplateSettingCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2431f0c265ab2acbfdd5efe0cfc9d3bfe4474dac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470305"
---
# <a name="update-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="d4e97-103">Atualizar deviceManagementTemplateSettingCategory</span><span class="sxs-lookup"><span data-stu-id="d4e97-103">Update deviceManagementTemplateSettingCategory</span></span>

<span data-ttu-id="d4e97-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d4e97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4e97-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4e97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4e97-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4e97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4e97-107">Atualiza as propriedades de um objeto [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="d4e97-107">Update the properties of a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4e97-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4e97-108">Prerequisites</span></span>
<span data-ttu-id="d4e97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4e97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4e97-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4e97-111">Permission type</span></span>|<span data-ttu-id="d4e97-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4e97-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4e97-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4e97-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4e97-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e97-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4e97-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4e97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4e97-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4e97-116">Not supported.</span></span>|
|<span data-ttu-id="d4e97-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4e97-117">Application</span></span>|<span data-ttu-id="d4e97-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e97-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4e97-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4e97-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="d4e97-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e97-120">Request headers</span></span>
|<span data-ttu-id="d4e97-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4e97-121">Header</span></span>|<span data-ttu-id="d4e97-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d4e97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4e97-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4e97-123">Authorization</span></span>|<span data-ttu-id="d4e97-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4e97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4e97-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4e97-125">Accept</span></span>|<span data-ttu-id="d4e97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4e97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4e97-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e97-127">Request body</span></span>
<span data-ttu-id="d4e97-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="d4e97-128">In the request body, supply a JSON representation for the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

<span data-ttu-id="d4e97-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="d4e97-129">The following table shows the properties that are required when you create the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md).</span></span>

|<span data-ttu-id="d4e97-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4e97-130">Property</span></span>|<span data-ttu-id="d4e97-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4e97-131">Type</span></span>|<span data-ttu-id="d4e97-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4e97-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4e97-133">id</span><span class="sxs-lookup"><span data-stu-id="d4e97-133">id</span></span>|<span data-ttu-id="d4e97-134">String</span><span class="sxs-lookup"><span data-stu-id="d4e97-134">String</span></span>|<span data-ttu-id="d4e97-135">A ID de categoria herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="d4e97-135">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="d4e97-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d4e97-136">displayName</span></span>|<span data-ttu-id="d4e97-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4e97-137">String</span></span>|<span data-ttu-id="d4e97-138">O nome da categoria herdado de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="d4e97-138">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="d4e97-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="d4e97-139">hasRequiredSetting</span></span>|<span data-ttu-id="d4e97-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e97-140">Boolean</span></span>|<span data-ttu-id="d4e97-141">A categoria contém a configuração necessária de nível superior herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="d4e97-141">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d4e97-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e97-142">Response</span></span>
<span data-ttu-id="d4e97-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e97-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4e97-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4e97-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4e97-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e97-145">Request</span></span>
<span data-ttu-id="d4e97-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4e97-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
Content-type: application/json
Content-length: 152

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="d4e97-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e97-147">Response</span></span>
<span data-ttu-id="d4e97-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4e97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 201

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "cd213562-3562-cd21-6235-21cd623521cd",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```





