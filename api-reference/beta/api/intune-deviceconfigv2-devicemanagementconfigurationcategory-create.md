---
title: Criar deviceManagementConfigurationCategory
description: Crie um novo objeto deviceManagementConfigurationCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cfaf2631a247bbfdf7ec884b69129fb17c5fb52f
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666433"
---
# <a name="create-devicemanagementconfigurationcategory"></a><span data-ttu-id="bbf71-103">Criar deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="bbf71-103">Create deviceManagementConfigurationCategory</span></span>

<span data-ttu-id="bbf71-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbf71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbf71-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bbf71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbf71-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bbf71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbf71-107">Crie um novo [objeto deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="bbf71-107">Create a new [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbf71-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bbf71-108">Prerequisites</span></span>
<span data-ttu-id="bbf71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbf71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbf71-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbf71-111">Permission type</span></span>|<span data-ttu-id="bbf71-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbf71-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbf71-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbf71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbf71-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf71-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bbf71-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbf71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbf71-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbf71-116">Not supported.</span></span>|
|<span data-ttu-id="bbf71-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbf71-117">Application</span></span>|<span data-ttu-id="bbf71-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf71-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbf71-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationCategories
```

## <a name="request-headers"></a><span data-ttu-id="bbf71-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf71-120">Request headers</span></span>
|<span data-ttu-id="bbf71-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbf71-121">Header</span></span>|<span data-ttu-id="bbf71-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bbf71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbf71-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbf71-123">Authorization</span></span>|<span data-ttu-id="bbf71-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbf71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbf71-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bbf71-125">Accept</span></span>|<span data-ttu-id="bbf71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbf71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbf71-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf71-127">Request body</span></span>
<span data-ttu-id="bbf71-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementConfigurationCategory.</span><span class="sxs-lookup"><span data-stu-id="bbf71-128">In the request body, supply a JSON representation for the deviceManagementConfigurationCategory object.</span></span>

<span data-ttu-id="bbf71-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationCategory.</span><span class="sxs-lookup"><span data-stu-id="bbf71-129">The following table shows the properties that are required when you create the deviceManagementConfigurationCategory.</span></span>

|<span data-ttu-id="bbf71-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbf71-130">Property</span></span>|<span data-ttu-id="bbf71-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbf71-131">Type</span></span>|<span data-ttu-id="bbf71-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbf71-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbf71-133">id</span><span class="sxs-lookup"><span data-stu-id="bbf71-133">id</span></span>|<span data-ttu-id="bbf71-134">String</span><span class="sxs-lookup"><span data-stu-id="bbf71-134">String</span></span>|<span data-ttu-id="bbf71-135">Identificador de item</span><span class="sxs-lookup"><span data-stu-id="bbf71-135">Identifier for item</span></span>|
|<span data-ttu-id="bbf71-136">descrição</span><span class="sxs-lookup"><span data-stu-id="bbf71-136">description</span></span>|<span data-ttu-id="bbf71-137">String</span><span class="sxs-lookup"><span data-stu-id="bbf71-137">String</span></span>|<span data-ttu-id="bbf71-138">Descrição do item</span><span class="sxs-lookup"><span data-stu-id="bbf71-138">Description of the item</span></span>|
|<span data-ttu-id="bbf71-139">helpText</span><span class="sxs-lookup"><span data-stu-id="bbf71-139">helpText</span></span>|<span data-ttu-id="bbf71-140">String</span><span class="sxs-lookup"><span data-stu-id="bbf71-140">String</span></span>|<span data-ttu-id="bbf71-141">Texto de ajuda do item</span><span class="sxs-lookup"><span data-stu-id="bbf71-141">Help text of the item</span></span>|
|<span data-ttu-id="bbf71-142">nome</span><span class="sxs-lookup"><span data-stu-id="bbf71-142">name</span></span>|<span data-ttu-id="bbf71-143">String</span><span class="sxs-lookup"><span data-stu-id="bbf71-143">String</span></span>|<span data-ttu-id="bbf71-144">Nome do item</span><span class="sxs-lookup"><span data-stu-id="bbf71-144">Name of the item</span></span>|
|<span data-ttu-id="bbf71-145">displayName</span><span class="sxs-lookup"><span data-stu-id="bbf71-145">displayName</span></span>|<span data-ttu-id="bbf71-146">String</span><span class="sxs-lookup"><span data-stu-id="bbf71-146">String</span></span>|<span data-ttu-id="bbf71-147">Nome de exibição do item</span><span class="sxs-lookup"><span data-stu-id="bbf71-147">Display name of the item</span></span>|
|<span data-ttu-id="bbf71-148">plataformas</span><span class="sxs-lookup"><span data-stu-id="bbf71-148">platforms</span></span>|[<span data-ttu-id="bbf71-149">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="bbf71-149">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="bbf71-150">Tipos de plataformas, que configurações na categoria têm.</span><span class="sxs-lookup"><span data-stu-id="bbf71-150">Platforms types, which settings in the category have.</span></span> <span data-ttu-id="bbf71-151">Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="bbf71-151">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="bbf71-152">technologies</span><span class="sxs-lookup"><span data-stu-id="bbf71-152">technologies</span></span>|[<span data-ttu-id="bbf71-153">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="bbf71-153">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="bbf71-154">Tipos de tecnologias, que configurações na categoria têm.</span><span class="sxs-lookup"><span data-stu-id="bbf71-154">Technologies types, which settings in the category have.</span></span> <span data-ttu-id="bbf71-155">Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span><span class="sxs-lookup"><span data-stu-id="bbf71-155">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|
|<span data-ttu-id="bbf71-156">settingUsage</span><span class="sxs-lookup"><span data-stu-id="bbf71-156">settingUsage</span></span>|[<span data-ttu-id="bbf71-157">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="bbf71-157">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="bbf71-158">Indica que a categoria contém configurações usadas para Conformidade ou Configuração.</span><span class="sxs-lookup"><span data-stu-id="bbf71-158">Indicates that the category contains settings that are used for Compliance or Configuration.</span></span> <span data-ttu-id="bbf71-159">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="bbf71-159">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="bbf71-160">parentCategoryId</span><span class="sxs-lookup"><span data-stu-id="bbf71-160">parentCategoryId</span></span>|<span data-ttu-id="bbf71-161">String</span><span class="sxs-lookup"><span data-stu-id="bbf71-161">String</span></span>|<span data-ttu-id="bbf71-162">ID pai da categoria.</span><span class="sxs-lookup"><span data-stu-id="bbf71-162">Parent id of the category.</span></span>|
|<span data-ttu-id="bbf71-163">rootCategoryId</span><span class="sxs-lookup"><span data-stu-id="bbf71-163">rootCategoryId</span></span>|<span data-ttu-id="bbf71-164">String</span><span class="sxs-lookup"><span data-stu-id="bbf71-164">String</span></span>|<span data-ttu-id="bbf71-165">ID raiz da categoria.</span><span class="sxs-lookup"><span data-stu-id="bbf71-165">Root id of the category.</span></span>|
|<span data-ttu-id="bbf71-166">childCategoryIds</span><span class="sxs-lookup"><span data-stu-id="bbf71-166">childCategoryIds</span></span>|<span data-ttu-id="bbf71-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbf71-167">String collection</span></span>|<span data-ttu-id="bbf71-168">Lista de IDs filho da categoria.</span><span class="sxs-lookup"><span data-stu-id="bbf71-168">List of child ids of the category.</span></span>|



## <a name="response"></a><span data-ttu-id="bbf71-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf71-169">Response</span></span>
<span data-ttu-id="bbf71-170">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbf71-170">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbf71-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbf71-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbf71-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf71-172">Request</span></span>
<span data-ttu-id="bbf71-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbf71-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationCategories
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

### <a name="response"></a><span data-ttu-id="bbf71-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf71-174">Response</span></span>
<span data-ttu-id="bbf71-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbf71-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




