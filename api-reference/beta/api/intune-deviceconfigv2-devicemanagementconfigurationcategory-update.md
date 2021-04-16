---
title: Atualizar deviceManagementConfigurationCategory
description: Atualize as propriedades de um objeto deviceManagementConfigurationCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b34323a883b24f9849f4b5d140f0dc0dc5faa08
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866269"
---
# <a name="update-devicemanagementconfigurationcategory"></a><span data-ttu-id="286d0-103">Atualizar deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="286d0-103">Update deviceManagementConfigurationCategory</span></span>

<span data-ttu-id="286d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="286d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="286d0-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="286d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="286d0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="286d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="286d0-107">Atualize as propriedades de [um objeto deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="286d0-107">Update the properties of a [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="286d0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="286d0-108">Prerequisites</span></span>
<span data-ttu-id="286d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="286d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="286d0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="286d0-111">Permission type</span></span>|<span data-ttu-id="286d0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="286d0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="286d0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="286d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="286d0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="286d0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="286d0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="286d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="286d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="286d0-116">Not supported.</span></span>|
|<span data-ttu-id="286d0-117">Application</span><span class="sxs-lookup"><span data-stu-id="286d0-117">Application</span></span>|<span data-ttu-id="286d0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="286d0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="286d0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="286d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="286d0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="286d0-120">Request headers</span></span>
|<span data-ttu-id="286d0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="286d0-121">Header</span></span>|<span data-ttu-id="286d0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="286d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="286d0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="286d0-123">Authorization</span></span>|<span data-ttu-id="286d0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="286d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="286d0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="286d0-125">Accept</span></span>|<span data-ttu-id="286d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="286d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="286d0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="286d0-127">Request body</span></span>
<span data-ttu-id="286d0-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="286d0-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

<span data-ttu-id="286d0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).</span><span class="sxs-lookup"><span data-stu-id="286d0-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).</span></span>

|<span data-ttu-id="286d0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="286d0-130">Property</span></span>|<span data-ttu-id="286d0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="286d0-131">Type</span></span>|<span data-ttu-id="286d0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="286d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="286d0-133">id</span><span class="sxs-lookup"><span data-stu-id="286d0-133">id</span></span>|<span data-ttu-id="286d0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="286d0-134">String</span></span>|<span data-ttu-id="286d0-135">Identificador de item</span><span class="sxs-lookup"><span data-stu-id="286d0-135">Identifier for item</span></span>|
|<span data-ttu-id="286d0-136">description</span><span class="sxs-lookup"><span data-stu-id="286d0-136">description</span></span>|<span data-ttu-id="286d0-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="286d0-137">String</span></span>|<span data-ttu-id="286d0-138">Descrição do item</span><span class="sxs-lookup"><span data-stu-id="286d0-138">Description of the item</span></span>|
|<span data-ttu-id="286d0-139">helpText</span><span class="sxs-lookup"><span data-stu-id="286d0-139">helpText</span></span>|<span data-ttu-id="286d0-140">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="286d0-140">String</span></span>|<span data-ttu-id="286d0-141">Texto de ajuda do item</span><span class="sxs-lookup"><span data-stu-id="286d0-141">Help text of the item</span></span>|
|<span data-ttu-id="286d0-142">nome</span><span class="sxs-lookup"><span data-stu-id="286d0-142">name</span></span>|<span data-ttu-id="286d0-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="286d0-143">String</span></span>|<span data-ttu-id="286d0-144">Nome do item</span><span class="sxs-lookup"><span data-stu-id="286d0-144">Name of the item</span></span>|
|<span data-ttu-id="286d0-145">displayName</span><span class="sxs-lookup"><span data-stu-id="286d0-145">displayName</span></span>|<span data-ttu-id="286d0-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="286d0-146">String</span></span>|<span data-ttu-id="286d0-147">Nome de exibição do item</span><span class="sxs-lookup"><span data-stu-id="286d0-147">Display name of the item</span></span>|
|<span data-ttu-id="286d0-148">plataformas</span><span class="sxs-lookup"><span data-stu-id="286d0-148">platforms</span></span>|[<span data-ttu-id="286d0-149">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="286d0-149">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="286d0-150">Tipos de plataformas, que configurações na categoria têm.</span><span class="sxs-lookup"><span data-stu-id="286d0-150">Platforms types, which settings in the category have.</span></span> <span data-ttu-id="286d0-151">Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="286d0-151">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="286d0-152">technologies</span><span class="sxs-lookup"><span data-stu-id="286d0-152">technologies</span></span>|[<span data-ttu-id="286d0-153">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="286d0-153">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="286d0-154">Tipos de tecnologias, que configurações na categoria têm.</span><span class="sxs-lookup"><span data-stu-id="286d0-154">Technologies types, which settings in the category have.</span></span> <span data-ttu-id="286d0-155">Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="286d0-155">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="286d0-156">settingUsage</span><span class="sxs-lookup"><span data-stu-id="286d0-156">settingUsage</span></span>|[<span data-ttu-id="286d0-157">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="286d0-157">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="286d0-158">Indica que a categoria contém configurações usadas para Conformidade ou Configuração.</span><span class="sxs-lookup"><span data-stu-id="286d0-158">Indicates that the category contains settings that are used for Compliance or Configuration.</span></span> <span data-ttu-id="286d0-159">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="286d0-159">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="286d0-160">parentCategoryId</span><span class="sxs-lookup"><span data-stu-id="286d0-160">parentCategoryId</span></span>|<span data-ttu-id="286d0-161">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="286d0-161">String</span></span>|<span data-ttu-id="286d0-162">ID pai da categoria.</span><span class="sxs-lookup"><span data-stu-id="286d0-162">Parent id of the category.</span></span>|
|<span data-ttu-id="286d0-163">rootCategoryId</span><span class="sxs-lookup"><span data-stu-id="286d0-163">rootCategoryId</span></span>|<span data-ttu-id="286d0-164">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="286d0-164">String</span></span>|<span data-ttu-id="286d0-165">ID raiz da categoria.</span><span class="sxs-lookup"><span data-stu-id="286d0-165">Root id of the category.</span></span>|
|<span data-ttu-id="286d0-166">childCategoryIds</span><span class="sxs-lookup"><span data-stu-id="286d0-166">childCategoryIds</span></span>|<span data-ttu-id="286d0-167">Coleção String</span><span class="sxs-lookup"><span data-stu-id="286d0-167">String collection</span></span>|<span data-ttu-id="286d0-168">Lista de IDs filho da categoria.</span><span class="sxs-lookup"><span data-stu-id="286d0-168">List of child ids of the category.</span></span>|



## <a name="response"></a><span data-ttu-id="286d0-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="286d0-169">Response</span></span>
<span data-ttu-id="286d0-170">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="286d0-170">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="286d0-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="286d0-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="286d0-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="286d0-172">Request</span></span>
<span data-ttu-id="286d0-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="286d0-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
Content-type: application/json
Content-length: 465

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "macOS",
  "technologies": "mdm",
  "settingUsage": "configuration",
  "parentCategoryId": "Parent Category Id value",
  "rootCategoryId": "Root Category Id value",
  "childCategoryIds": [
    "Child Category Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="286d0-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="286d0-174">Response</span></span>
<span data-ttu-id="286d0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="286d0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 514

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "cff34dd2-4dd2-cff3-d24d-f3cfd24df3cf",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "macOS",
  "technologies": "mdm",
  "settingUsage": "configuration",
  "parentCategoryId": "Parent Category Id value",
  "rootCategoryId": "Root Category Id value",
  "childCategoryIds": [
    "Child Category Ids value"
  ]
}
```




