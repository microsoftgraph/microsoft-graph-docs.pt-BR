---
title: Criar deviceManagementConfigurationPolicy
description: Crie um novo objeto deviceManagementConfigurationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 94410b8e7b3259a74893e93b450486398c5bef13
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129269"
---
# <a name="create-devicemanagementconfigurationpolicy"></a><span data-ttu-id="9bb6c-103">Criar deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="9bb6c-103">Create deviceManagementConfigurationPolicy</span></span>

<span data-ttu-id="9bb6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bb6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bb6c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bb6c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bb6c-107">Crie um novo [objeto deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9bb6c-107">Create a new [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bb6c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9bb6c-108">Prerequisites</span></span>
<span data-ttu-id="9bb6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bb6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bb6c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bb6c-111">Permission type</span></span>|<span data-ttu-id="9bb6c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9bb6c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bb6c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bb6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bb6c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bb6c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9bb6c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bb6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bb6c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-116">Not supported.</span></span>|
|<span data-ttu-id="9bb6c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bb6c-117">Application</span></span>|<span data-ttu-id="9bb6c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bb6c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bb6c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bb6c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies
```

## <a name="request-headers"></a><span data-ttu-id="9bb6c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bb6c-120">Request headers</span></span>
|<span data-ttu-id="9bb6c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bb6c-121">Header</span></span>|<span data-ttu-id="9bb6c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9bb6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bb6c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bb6c-123">Authorization</span></span>|<span data-ttu-id="9bb6c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bb6c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9bb6c-125">Accept</span></span>|<span data-ttu-id="9bb6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bb6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bb6c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bb6c-127">Request body</span></span>
<span data-ttu-id="9bb6c-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementConfigurationPolicy.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-128">In the request body, supply a JSON representation for the deviceManagementConfigurationPolicy object.</span></span>

<span data-ttu-id="9bb6c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationPolicy.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-129">The following table shows the properties that are required when you create the deviceManagementConfigurationPolicy.</span></span>

|<span data-ttu-id="9bb6c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bb6c-130">Property</span></span>|<span data-ttu-id="9bb6c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bb6c-131">Type</span></span>|<span data-ttu-id="9bb6c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bb6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bb6c-133">id</span><span class="sxs-lookup"><span data-stu-id="9bb6c-133">id</span></span>|<span data-ttu-id="9bb6c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb6c-134">String</span></span>|<span data-ttu-id="9bb6c-135">Chave do documento de política.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-135">Key of the policy document.</span></span> <span data-ttu-id="9bb6c-136">Gerado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-136">Automatically generated.</span></span>|
|<span data-ttu-id="9bb6c-137">nome</span><span class="sxs-lookup"><span data-stu-id="9bb6c-137">name</span></span>|<span data-ttu-id="9bb6c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb6c-138">String</span></span>|<span data-ttu-id="9bb6c-139">Nome da política</span><span class="sxs-lookup"><span data-stu-id="9bb6c-139">Policy name</span></span>|
|<span data-ttu-id="9bb6c-140">descrição</span><span class="sxs-lookup"><span data-stu-id="9bb6c-140">description</span></span>|<span data-ttu-id="9bb6c-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb6c-141">String</span></span>|<span data-ttu-id="9bb6c-142">Descrição da política</span><span class="sxs-lookup"><span data-stu-id="9bb6c-142">Policy description</span></span>|
|<span data-ttu-id="9bb6c-143">plataformas</span><span class="sxs-lookup"><span data-stu-id="9bb6c-143">platforms</span></span>|[<span data-ttu-id="9bb6c-144">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="9bb6c-144">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="9bb6c-145">Plataformas para essa política.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-145">Platforms for this policy.</span></span> <span data-ttu-id="9bb6c-146">Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-146">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="9bb6c-147">technologies</span><span class="sxs-lookup"><span data-stu-id="9bb6c-147">technologies</span></span>|[<span data-ttu-id="9bb6c-148">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="9bb6c-148">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="9bb6c-149">Tecnologias para essa política.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-149">Technologies for this policy.</span></span> <span data-ttu-id="9bb6c-150">Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-150">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="9bb6c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9bb6c-151">createdDateTime</span></span>|<span data-ttu-id="9bb6c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bb6c-152">DateTimeOffset</span></span>|<span data-ttu-id="9bb6c-153">Data e hora de criação de política.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-153">Policy creation date and time.</span></span> <span data-ttu-id="9bb6c-154">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-154">This property is read-only.</span></span>|
|<span data-ttu-id="9bb6c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9bb6c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="9bb6c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bb6c-156">DateTimeOffset</span></span>|<span data-ttu-id="9bb6c-157">Data e hora da última modificação da política.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-157">Policy last modification date and time.</span></span> <span data-ttu-id="9bb6c-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-158">This property is read-only.</span></span>|
|<span data-ttu-id="9bb6c-159">settingCount</span><span class="sxs-lookup"><span data-stu-id="9bb6c-159">settingCount</span></span>|<span data-ttu-id="9bb6c-160">Int32</span><span class="sxs-lookup"><span data-stu-id="9bb6c-160">Int32</span></span>|<span data-ttu-id="9bb6c-161">Número de configurações.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-161">Number of settings.</span></span> <span data-ttu-id="9bb6c-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-162">This property is read-only.</span></span>|
|<span data-ttu-id="9bb6c-163">creationSource</span><span class="sxs-lookup"><span data-stu-id="9bb6c-163">creationSource</span></span>|<span data-ttu-id="9bb6c-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb6c-164">String</span></span>|<span data-ttu-id="9bb6c-165">Fonte de criação de política</span><span class="sxs-lookup"><span data-stu-id="9bb6c-165">Policy creation source</span></span>|
|<span data-ttu-id="9bb6c-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9bb6c-166">roleScopeTagIds</span></span>|<span data-ttu-id="9bb6c-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb6c-167">String collection</span></span>|<span data-ttu-id="9bb6c-168">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-168">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="9bb6c-169">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9bb6c-169">isAssigned</span></span>|<span data-ttu-id="9bb6c-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bb6c-170">Boolean</span></span>|<span data-ttu-id="9bb6c-171">Status da atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-171">Policy assignment status.</span></span> <span data-ttu-id="9bb6c-172">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-172">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="9bb6c-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bb6c-173">Response</span></span>
<span data-ttu-id="9bb6c-174">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-174">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bb6c-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bb6c-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bb6c-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bb6c-176">Request</span></span>
<span data-ttu-id="9bb6c-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies
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

### <a name="response"></a><span data-ttu-id="9bb6c-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bb6c-178">Response</span></span>
<span data-ttu-id="9bb6c-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bb6c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




