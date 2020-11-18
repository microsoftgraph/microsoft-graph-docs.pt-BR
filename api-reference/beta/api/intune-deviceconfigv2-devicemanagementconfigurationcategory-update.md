---
title: Atualizar deviceManagementConfigurationCategory
description: Atualiza as propriedades de um objeto deviceManagementConfigurationCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e695f9935905d781d7d6ca3e8a8e36f1cfc36c74
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241125"
---
# <a name="update-devicemanagementconfigurationcategory"></a><span data-ttu-id="56a78-103">Atualizar deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="56a78-103">Update deviceManagementConfigurationCategory</span></span>

<span data-ttu-id="56a78-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56a78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56a78-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56a78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56a78-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56a78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56a78-107">Atualiza as propriedades de um objeto [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="56a78-107">Update the properties of a [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56a78-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56a78-108">Prerequisites</span></span>
<span data-ttu-id="56a78-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56a78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56a78-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56a78-111">Permission type</span></span>|<span data-ttu-id="56a78-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56a78-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56a78-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56a78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56a78-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56a78-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56a78-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56a78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56a78-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56a78-116">Not supported.</span></span>|
|<span data-ttu-id="56a78-117">Application</span><span class="sxs-lookup"><span data-stu-id="56a78-117">Application</span></span>|<span data-ttu-id="56a78-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56a78-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56a78-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56a78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="56a78-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56a78-120">Request headers</span></span>
|<span data-ttu-id="56a78-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56a78-121">Header</span></span>|<span data-ttu-id="56a78-122">Valor</span><span class="sxs-lookup"><span data-stu-id="56a78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56a78-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="56a78-123">Authorization</span></span>|<span data-ttu-id="56a78-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56a78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56a78-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56a78-125">Accept</span></span>|<span data-ttu-id="56a78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56a78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56a78-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56a78-127">Request body</span></span>
<span data-ttu-id="56a78-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="56a78-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

<span data-ttu-id="56a78-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).</span><span class="sxs-lookup"><span data-stu-id="56a78-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).</span></span>

|<span data-ttu-id="56a78-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56a78-130">Property</span></span>|<span data-ttu-id="56a78-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="56a78-131">Type</span></span>|<span data-ttu-id="56a78-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="56a78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56a78-133">id</span><span class="sxs-lookup"><span data-stu-id="56a78-133">id</span></span>|<span data-ttu-id="56a78-134">String</span><span class="sxs-lookup"><span data-stu-id="56a78-134">String</span></span>|<span data-ttu-id="56a78-135">Identificador do item</span><span class="sxs-lookup"><span data-stu-id="56a78-135">Identifier for item</span></span>|
|<span data-ttu-id="56a78-136">description</span><span class="sxs-lookup"><span data-stu-id="56a78-136">description</span></span>|<span data-ttu-id="56a78-137">String</span><span class="sxs-lookup"><span data-stu-id="56a78-137">String</span></span>|<span data-ttu-id="56a78-138">Descrição do item</span><span class="sxs-lookup"><span data-stu-id="56a78-138">Description of the item</span></span>|
|<span data-ttu-id="56a78-139">helpText</span><span class="sxs-lookup"><span data-stu-id="56a78-139">helpText</span></span>|<span data-ttu-id="56a78-140">String</span><span class="sxs-lookup"><span data-stu-id="56a78-140">String</span></span>|<span data-ttu-id="56a78-141">Texto de ajuda do item</span><span class="sxs-lookup"><span data-stu-id="56a78-141">Help text of the item</span></span>|
|<span data-ttu-id="56a78-142">nome</span><span class="sxs-lookup"><span data-stu-id="56a78-142">name</span></span>|<span data-ttu-id="56a78-143">String</span><span class="sxs-lookup"><span data-stu-id="56a78-143">String</span></span>|<span data-ttu-id="56a78-144">Nome do item</span><span class="sxs-lookup"><span data-stu-id="56a78-144">Name of the item</span></span>|
|<span data-ttu-id="56a78-145">displayName</span><span class="sxs-lookup"><span data-stu-id="56a78-145">displayName</span></span>|<span data-ttu-id="56a78-146">String</span><span class="sxs-lookup"><span data-stu-id="56a78-146">String</span></span>|<span data-ttu-id="56a78-147">Nome para exibição do item</span><span class="sxs-lookup"><span data-stu-id="56a78-147">Display name of the item</span></span>|
|<span data-ttu-id="56a78-148">plataformas</span><span class="sxs-lookup"><span data-stu-id="56a78-148">platforms</span></span>|[<span data-ttu-id="56a78-149">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="56a78-149">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="56a78-150">Tipos de plataformas, quais configurações na categoria têm.</span><span class="sxs-lookup"><span data-stu-id="56a78-150">Platforms types, which settings in the category have.</span></span> <span data-ttu-id="56a78-151">Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="56a78-151">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="56a78-152">tecnologias</span><span class="sxs-lookup"><span data-stu-id="56a78-152">technologies</span></span>|[<span data-ttu-id="56a78-153">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="56a78-153">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="56a78-154">Tipos de tecnologias, as configurações na categoria têm.</span><span class="sxs-lookup"><span data-stu-id="56a78-154">Technologies types, which settings in the category have.</span></span> <span data-ttu-id="56a78-155">Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="56a78-155">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|



## <a name="response"></a><span data-ttu-id="56a78-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="56a78-156">Response</span></span>
<span data-ttu-id="56a78-157">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56a78-157">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56a78-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56a78-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="56a78-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56a78-159">Request</span></span>
<span data-ttu-id="56a78-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56a78-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
Content-type: application/json
Content-length: 268

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "macOS",
  "technologies": "mdm"
}
```

### <a name="response"></a><span data-ttu-id="56a78-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="56a78-161">Response</span></span>
<span data-ttu-id="56a78-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56a78-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "cff34dd2-4dd2-cff3-d24d-f3cfd24df3cf",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "macOS",
  "technologies": "mdm"
}
```




