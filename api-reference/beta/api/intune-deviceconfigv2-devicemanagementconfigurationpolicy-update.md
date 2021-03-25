---
title: Atualizar deviceManagementConfigurationPolicy
description: Atualize as propriedades de um objeto deviceManagementConfigurationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 68cc244764c3675145ea2019678ddc61af873db8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150875"
---
# <a name="update-devicemanagementconfigurationpolicy"></a><span data-ttu-id="12093-103">Atualizar deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="12093-103">Update deviceManagementConfigurationPolicy</span></span>

<span data-ttu-id="12093-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12093-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12093-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12093-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12093-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12093-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12093-107">Atualize as propriedades de [um objeto deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12093-107">Update the properties of a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12093-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12093-108">Prerequisites</span></span>
<span data-ttu-id="12093-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12093-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12093-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12093-111">Permission type</span></span>|<span data-ttu-id="12093-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12093-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12093-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12093-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12093-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12093-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12093-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12093-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12093-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12093-116">Not supported.</span></span>|
|<span data-ttu-id="12093-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12093-117">Application</span></span>|<span data-ttu-id="12093-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12093-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12093-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12093-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="12093-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12093-120">Request headers</span></span>
|<span data-ttu-id="12093-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12093-121">Header</span></span>|<span data-ttu-id="12093-122">Valor</span><span class="sxs-lookup"><span data-stu-id="12093-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12093-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="12093-123">Authorization</span></span>|<span data-ttu-id="12093-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12093-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12093-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12093-125">Accept</span></span>|<span data-ttu-id="12093-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12093-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12093-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12093-127">Request body</span></span>
<span data-ttu-id="12093-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12093-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

<span data-ttu-id="12093-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="12093-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md).</span></span>

|<span data-ttu-id="12093-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12093-130">Property</span></span>|<span data-ttu-id="12093-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="12093-131">Type</span></span>|<span data-ttu-id="12093-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="12093-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12093-133">id</span><span class="sxs-lookup"><span data-stu-id="12093-133">id</span></span>|<span data-ttu-id="12093-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12093-134">String</span></span>|<span data-ttu-id="12093-135">Chave do documento de política.</span><span class="sxs-lookup"><span data-stu-id="12093-135">Key of the policy document.</span></span> <span data-ttu-id="12093-136">Gerado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="12093-136">Automatically generated.</span></span>|
|<span data-ttu-id="12093-137">nome</span><span class="sxs-lookup"><span data-stu-id="12093-137">name</span></span>|<span data-ttu-id="12093-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12093-138">String</span></span>|<span data-ttu-id="12093-139">Nome da política</span><span class="sxs-lookup"><span data-stu-id="12093-139">Policy name</span></span>|
|<span data-ttu-id="12093-140">descrição</span><span class="sxs-lookup"><span data-stu-id="12093-140">description</span></span>|<span data-ttu-id="12093-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12093-141">String</span></span>|<span data-ttu-id="12093-142">Descrição da política</span><span class="sxs-lookup"><span data-stu-id="12093-142">Policy description</span></span>|
|<span data-ttu-id="12093-143">plataformas</span><span class="sxs-lookup"><span data-stu-id="12093-143">platforms</span></span>|[<span data-ttu-id="12093-144">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="12093-144">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="12093-145">Plataformas para essa política.</span><span class="sxs-lookup"><span data-stu-id="12093-145">Platforms for this policy.</span></span> <span data-ttu-id="12093-146">Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="12093-146">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="12093-147">technologies</span><span class="sxs-lookup"><span data-stu-id="12093-147">technologies</span></span>|[<span data-ttu-id="12093-148">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="12093-148">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="12093-149">Tecnologias para essa política.</span><span class="sxs-lookup"><span data-stu-id="12093-149">Technologies for this policy.</span></span> <span data-ttu-id="12093-150">Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="12093-150">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="12093-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12093-151">createdDateTime</span></span>|<span data-ttu-id="12093-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12093-152">DateTimeOffset</span></span>|<span data-ttu-id="12093-153">Data e hora de criação de política.</span><span class="sxs-lookup"><span data-stu-id="12093-153">Policy creation date and time.</span></span> <span data-ttu-id="12093-154">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12093-154">This property is read-only.</span></span>|
|<span data-ttu-id="12093-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12093-155">lastModifiedDateTime</span></span>|<span data-ttu-id="12093-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12093-156">DateTimeOffset</span></span>|<span data-ttu-id="12093-157">Data e hora da última modificação da política.</span><span class="sxs-lookup"><span data-stu-id="12093-157">Policy last modification date and time.</span></span> <span data-ttu-id="12093-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12093-158">This property is read-only.</span></span>|
|<span data-ttu-id="12093-159">settingCount</span><span class="sxs-lookup"><span data-stu-id="12093-159">settingCount</span></span>|<span data-ttu-id="12093-160">Int32</span><span class="sxs-lookup"><span data-stu-id="12093-160">Int32</span></span>|<span data-ttu-id="12093-161">Número de configurações.</span><span class="sxs-lookup"><span data-stu-id="12093-161">Number of settings.</span></span> <span data-ttu-id="12093-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12093-162">This property is read-only.</span></span>|
|<span data-ttu-id="12093-163">creationSource</span><span class="sxs-lookup"><span data-stu-id="12093-163">creationSource</span></span>|<span data-ttu-id="12093-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12093-164">String</span></span>|<span data-ttu-id="12093-165">Fonte de criação de política</span><span class="sxs-lookup"><span data-stu-id="12093-165">Policy creation source</span></span>|
|<span data-ttu-id="12093-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12093-166">roleScopeTagIds</span></span>|<span data-ttu-id="12093-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="12093-167">String collection</span></span>|<span data-ttu-id="12093-168">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="12093-168">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="12093-169">isAssigned</span><span class="sxs-lookup"><span data-stu-id="12093-169">isAssigned</span></span>|<span data-ttu-id="12093-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="12093-170">Boolean</span></span>|<span data-ttu-id="12093-171">Status da atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="12093-171">Policy assignment status.</span></span> <span data-ttu-id="12093-172">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12093-172">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="12093-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="12093-173">Response</span></span>
<span data-ttu-id="12093-174">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12093-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12093-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12093-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="12093-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12093-176">Request</span></span>
<span data-ttu-id="12093-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12093-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}
Content-type: application/json
Content-length: 346

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "name": "Name value",
  "description": "Description value",
  "platforms": "macOS",
  "technologies": "mdm",
  "settingCount": 12,
  "creationSource": "Creation Source value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="12093-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="12093-178">Response</span></span>
<span data-ttu-id="12093-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12093-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "id": "3ffd7cd0-7cd0-3ffd-d07c-fd3fd07cfd3f",
  "name": "Name value",
  "description": "Description value",
  "platforms": "macOS",
  "technologies": "mdm",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "settingCount": 12,
  "creationSource": "Creation Source value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isAssigned": true
}
```




