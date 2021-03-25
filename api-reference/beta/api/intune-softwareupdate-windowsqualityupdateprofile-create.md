---
title: Criar windowsQualityUpdateProfile
description: Crie um novo objeto windowsQualityUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 19a6a9c7b267ad4de2e675a43f5fd5420736a5c6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156244"
---
# <a name="create-windowsqualityupdateprofile"></a><span data-ttu-id="0b022-103">Criar windowsQualityUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="0b022-103">Create windowsQualityUpdateProfile</span></span>

<span data-ttu-id="0b022-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b022-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b022-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b022-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b022-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b022-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b022-107">Crie um novo [objeto windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0b022-107">Create a new [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b022-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b022-108">Prerequisites</span></span>
<span data-ttu-id="0b022-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b022-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b022-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b022-111">Permission type</span></span>|<span data-ttu-id="0b022-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b022-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b022-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b022-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b022-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b022-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b022-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b022-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b022-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b022-116">Not supported.</span></span>|
|<span data-ttu-id="0b022-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b022-117">Application</span></span>|<span data-ttu-id="0b022-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b022-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b022-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b022-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsQualityUpdateProfiles
```

## <a name="request-headers"></a><span data-ttu-id="0b022-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b022-120">Request headers</span></span>
|<span data-ttu-id="0b022-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b022-121">Header</span></span>|<span data-ttu-id="0b022-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0b022-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b022-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b022-123">Authorization</span></span>|<span data-ttu-id="0b022-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b022-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b022-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b022-125">Accept</span></span>|<span data-ttu-id="0b022-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b022-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b022-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b022-127">Request body</span></span>
<span data-ttu-id="0b022-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsQualityUpdateProfile.</span><span class="sxs-lookup"><span data-stu-id="0b022-128">In the request body, supply a JSON representation for the windowsQualityUpdateProfile object.</span></span>

<span data-ttu-id="0b022-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsQualityUpdateProfile.</span><span class="sxs-lookup"><span data-stu-id="0b022-129">The following table shows the properties that are required when you create the windowsQualityUpdateProfile.</span></span>

|<span data-ttu-id="0b022-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b022-130">Property</span></span>|<span data-ttu-id="0b022-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b022-131">Type</span></span>|<span data-ttu-id="0b022-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b022-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b022-133">id</span><span class="sxs-lookup"><span data-stu-id="0b022-133">id</span></span>|<span data-ttu-id="0b022-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b022-134">String</span></span>|<span data-ttu-id="0b022-135">A ID da política do Intune.</span><span class="sxs-lookup"><span data-stu-id="0b022-135">The Intune policy id.</span></span>|
|<span data-ttu-id="0b022-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0b022-136">displayName</span></span>|<span data-ttu-id="0b022-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b022-137">String</span></span>|<span data-ttu-id="0b022-138">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="0b022-138">The display name for the profile.</span></span>|
|<span data-ttu-id="0b022-139">descrição</span><span class="sxs-lookup"><span data-stu-id="0b022-139">description</span></span>|<span data-ttu-id="0b022-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b022-140">String</span></span>|<span data-ttu-id="0b022-141">A descrição do perfil especificado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="0b022-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="0b022-142">expeditedUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="0b022-142">expeditedUpdateSettings</span></span>|[<span data-ttu-id="0b022-143">expeditedWindowsQualityUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="0b022-143">expeditedWindowsQualityUpdateSettings</span></span>](../resources/intune-softwareupdate-expeditedwindowsqualityupdatesettings.md)|<span data-ttu-id="0b022-144">Configurações de atualização aceleradas.</span><span class="sxs-lookup"><span data-stu-id="0b022-144">Expedited update settings.</span></span>|
|<span data-ttu-id="0b022-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b022-145">createdDateTime</span></span>|<span data-ttu-id="0b022-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b022-146">DateTimeOffset</span></span>|<span data-ttu-id="0b022-147">A data em que o perfil foi criado.</span><span class="sxs-lookup"><span data-stu-id="0b022-147">The date time that the profile was created.</span></span>|
|<span data-ttu-id="0b022-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b022-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0b022-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b022-149">DateTimeOffset</span></span>|<span data-ttu-id="0b022-150">A data em que o perfil foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0b022-150">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="0b022-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0b022-151">roleScopeTagIds</span></span>|<span data-ttu-id="0b022-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b022-152">String collection</span></span>|<span data-ttu-id="0b022-153">Lista de Marcas de Escopo para esta entidade de Atualização de Qualidade.</span><span class="sxs-lookup"><span data-stu-id="0b022-153">List of Scope Tags for this Quality Update entity.</span></span>|
|<span data-ttu-id="0b022-154">releaseDateDisplayName</span><span class="sxs-lookup"><span data-stu-id="0b022-154">releaseDateDisplayName</span></span>|<span data-ttu-id="0b022-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b022-155">String</span></span>|<span data-ttu-id="0b022-156">Data de lançamento amigável a ser exibida para um lançamento de Atualização de Qualidade</span><span class="sxs-lookup"><span data-stu-id="0b022-156">Friendly release date to display for a Quality Update release</span></span>|
|<span data-ttu-id="0b022-157">deployableContentDisplayName</span><span class="sxs-lookup"><span data-stu-id="0b022-157">deployableContentDisplayName</span></span>|<span data-ttu-id="0b022-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b022-158">String</span></span>|<span data-ttu-id="0b022-159">Nome de exibição amigável do conteúdo implantável do perfil de atualização de qualidade</span><span class="sxs-lookup"><span data-stu-id="0b022-159">Friendly display name of the quality update profile deployable content</span></span>|



## <a name="response"></a><span data-ttu-id="0b022-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b022-160">Response</span></span>
<span data-ttu-id="0b022-161">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b022-161">If successful, this method returns a `201 Created` response code and a [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b022-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b022-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b022-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b022-163">Request</span></span>
<span data-ttu-id="0b022-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b022-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles
Content-type: application/json
Content-length: 558

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "expeditedUpdateSettings": {
    "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
    "qualityUpdateRelease": "Quality Update Release value",
    "daysUntilForcedReboot": 5
  },
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "releaseDateDisplayName": "Release Date Display Name value",
  "deployableContentDisplayName": "Deployable Content Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="0b022-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b022-165">Response</span></span>
<span data-ttu-id="0b022-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b022-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 730

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
  "id": "76fc7b65-7b65-76fc-657b-fc76657bfc76",
  "displayName": "Display Name value",
  "description": "Description value",
  "expeditedUpdateSettings": {
    "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
    "qualityUpdateRelease": "Quality Update Release value",
    "daysUntilForcedReboot": 5
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "releaseDateDisplayName": "Release Date Display Name value",
  "deployableContentDisplayName": "Deployable Content Display Name value"
}
```




