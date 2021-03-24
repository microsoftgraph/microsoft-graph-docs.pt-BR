---
title: Criar windowsFeatureUpdateProfile
description: Crie um novo objeto windowsFeatureUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83decaf1a8e8721cce6b23480626dcabfcbb5f36
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134281"
---
# <a name="create-windowsfeatureupdateprofile"></a><span data-ttu-id="535e0-103">Criar windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="535e0-103">Create windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="535e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="535e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="535e0-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="535e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="535e0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="535e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="535e0-107">Crie um novo [objeto windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="535e0-107">Create a new [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="535e0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="535e0-108">Prerequisites</span></span>
<span data-ttu-id="535e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="535e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="535e0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="535e0-111">Permission type</span></span>|<span data-ttu-id="535e0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="535e0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="535e0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="535e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="535e0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="535e0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="535e0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="535e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="535e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="535e0-116">Not supported.</span></span>|
|<span data-ttu-id="535e0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="535e0-117">Application</span></span>|<span data-ttu-id="535e0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="535e0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="535e0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="535e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles
```

## <a name="request-headers"></a><span data-ttu-id="535e0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="535e0-120">Request headers</span></span>
|<span data-ttu-id="535e0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="535e0-121">Header</span></span>|<span data-ttu-id="535e0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="535e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="535e0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="535e0-123">Authorization</span></span>|<span data-ttu-id="535e0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="535e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="535e0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="535e0-125">Accept</span></span>|<span data-ttu-id="535e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="535e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="535e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="535e0-127">Request body</span></span>
<span data-ttu-id="535e0-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsFeatureUpdateProfile.</span><span class="sxs-lookup"><span data-stu-id="535e0-128">In the request body, supply a JSON representation for the windowsFeatureUpdateProfile object.</span></span>

<span data-ttu-id="535e0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsFeatureUpdateProfile.</span><span class="sxs-lookup"><span data-stu-id="535e0-129">The following table shows the properties that are required when you create the windowsFeatureUpdateProfile.</span></span>

|<span data-ttu-id="535e0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="535e0-130">Property</span></span>|<span data-ttu-id="535e0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="535e0-131">Type</span></span>|<span data-ttu-id="535e0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="535e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="535e0-133">id</span><span class="sxs-lookup"><span data-stu-id="535e0-133">id</span></span>|<span data-ttu-id="535e0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="535e0-134">String</span></span>|<span data-ttu-id="535e0-135">O Identificador da entidade.</span><span class="sxs-lookup"><span data-stu-id="535e0-135">The Identifier of the entity.</span></span>|
|<span data-ttu-id="535e0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="535e0-136">displayName</span></span>|<span data-ttu-id="535e0-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="535e0-137">String</span></span>|<span data-ttu-id="535e0-138">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="535e0-138">The display name of the profile.</span></span>|
|<span data-ttu-id="535e0-139">descrição</span><span class="sxs-lookup"><span data-stu-id="535e0-139">description</span></span>|<span data-ttu-id="535e0-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="535e0-140">String</span></span>|<span data-ttu-id="535e0-141">A descrição do perfil especificado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="535e0-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="535e0-142">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="535e0-142">featureUpdateVersion</span></span>|<span data-ttu-id="535e0-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="535e0-143">String</span></span>|<span data-ttu-id="535e0-144">A versão de atualização de recursos que será implantada nos dispositivos direcionados por esse perfil.</span><span class="sxs-lookup"><span data-stu-id="535e0-144">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="535e0-145">A versão pode ser qualquer versão com suporte para o exemplo 1709, 1803 ou 1809 e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="535e0-145">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="535e0-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="535e0-146">createdDateTime</span></span>|<span data-ttu-id="535e0-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="535e0-147">DateTimeOffset</span></span>|<span data-ttu-id="535e0-148">A data em que o perfil foi criado.</span><span class="sxs-lookup"><span data-stu-id="535e0-148">The date time that the profile was created.</span></span>|
|<span data-ttu-id="535e0-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="535e0-149">lastModifiedDateTime</span></span>|<span data-ttu-id="535e0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="535e0-150">DateTimeOffset</span></span>|<span data-ttu-id="535e0-151">A data em que o perfil foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="535e0-151">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="535e0-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="535e0-152">roleScopeTagIds</span></span>|<span data-ttu-id="535e0-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="535e0-153">String collection</span></span>|<span data-ttu-id="535e0-154">Lista de Marcas de Escopo para essa entidade atualização de recursos.</span><span class="sxs-lookup"><span data-stu-id="535e0-154">List of Scope Tags for this Feature Update entity.</span></span>|
|<span data-ttu-id="535e0-155">deployableContentDisplayName</span><span class="sxs-lookup"><span data-stu-id="535e0-155">deployableContentDisplayName</span></span>|<span data-ttu-id="535e0-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="535e0-156">String</span></span>|<span data-ttu-id="535e0-157">Nome de exibição amigável do conteúdo implantável do perfil de atualização de qualidade</span><span class="sxs-lookup"><span data-stu-id="535e0-157">Friendly display name of the quality update profile deployable content</span></span>|



## <a name="response"></a><span data-ttu-id="535e0-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="535e0-158">Response</span></span>
<span data-ttu-id="535e0-159">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="535e0-159">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="535e0-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="535e0-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="535e0-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="535e0-161">Request</span></span>
<span data-ttu-id="535e0-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="535e0-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles
Content-type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deployableContentDisplayName": "Deployable Content Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="535e0-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="535e0-163">Response</span></span>
<span data-ttu-id="535e0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="535e0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 517

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deployableContentDisplayName": "Deployable Content Display Name value"
}
```




