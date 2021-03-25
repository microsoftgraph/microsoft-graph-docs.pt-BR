---
title: Atualizar windowsQualityUpdateProfile
description: Atualize as propriedades de um objeto windowsQualityUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62932ae10bc64ecf63ece2648527d7babad8731e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156174"
---
# <a name="update-windowsqualityupdateprofile"></a><span data-ttu-id="3d576-103">Atualizar windowsQualityUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="3d576-103">Update windowsQualityUpdateProfile</span></span>

<span data-ttu-id="3d576-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d576-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d576-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3d576-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d576-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d576-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d576-107">Atualize as propriedades de um [objeto windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3d576-107">Update the properties of a [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d576-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3d576-108">Prerequisites</span></span>
<span data-ttu-id="3d576-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d576-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d576-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d576-111">Permission type</span></span>|<span data-ttu-id="3d576-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d576-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d576-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d576-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d576-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d576-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3d576-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d576-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d576-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d576-116">Not supported.</span></span>|
|<span data-ttu-id="3d576-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d576-117">Application</span></span>|<span data-ttu-id="3d576-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d576-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d576-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d576-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="3d576-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d576-120">Request headers</span></span>
|<span data-ttu-id="3d576-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3d576-121">Header</span></span>|<span data-ttu-id="3d576-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3d576-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d576-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d576-123">Authorization</span></span>|<span data-ttu-id="3d576-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d576-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d576-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3d576-125">Accept</span></span>|<span data-ttu-id="3d576-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d576-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d576-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d576-127">Request body</span></span>
<span data-ttu-id="3d576-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3d576-128">In the request body, supply a JSON representation for the [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object.</span></span>

<span data-ttu-id="3d576-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="3d576-129">The following table shows the properties that are required when you create the [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md).</span></span>

|<span data-ttu-id="3d576-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d576-130">Property</span></span>|<span data-ttu-id="3d576-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d576-131">Type</span></span>|<span data-ttu-id="3d576-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d576-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d576-133">id</span><span class="sxs-lookup"><span data-stu-id="3d576-133">id</span></span>|<span data-ttu-id="3d576-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d576-134">String</span></span>|<span data-ttu-id="3d576-135">A ID da política do Intune.</span><span class="sxs-lookup"><span data-stu-id="3d576-135">The Intune policy id.</span></span>|
|<span data-ttu-id="3d576-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3d576-136">displayName</span></span>|<span data-ttu-id="3d576-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d576-137">String</span></span>|<span data-ttu-id="3d576-138">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="3d576-138">The display name for the profile.</span></span>|
|<span data-ttu-id="3d576-139">descrição</span><span class="sxs-lookup"><span data-stu-id="3d576-139">description</span></span>|<span data-ttu-id="3d576-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d576-140">String</span></span>|<span data-ttu-id="3d576-141">A descrição do perfil especificado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="3d576-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="3d576-142">expeditedUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="3d576-142">expeditedUpdateSettings</span></span>|[<span data-ttu-id="3d576-143">expeditedWindowsQualityUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="3d576-143">expeditedWindowsQualityUpdateSettings</span></span>](../resources/intune-softwareupdate-expeditedwindowsqualityupdatesettings.md)|<span data-ttu-id="3d576-144">Configurações de atualização aceleradas.</span><span class="sxs-lookup"><span data-stu-id="3d576-144">Expedited update settings.</span></span>|
|<span data-ttu-id="3d576-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d576-145">createdDateTime</span></span>|<span data-ttu-id="3d576-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d576-146">DateTimeOffset</span></span>|<span data-ttu-id="3d576-147">A data em que o perfil foi criado.</span><span class="sxs-lookup"><span data-stu-id="3d576-147">The date time that the profile was created.</span></span>|
|<span data-ttu-id="3d576-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d576-148">lastModifiedDateTime</span></span>|<span data-ttu-id="3d576-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d576-149">DateTimeOffset</span></span>|<span data-ttu-id="3d576-150">A data em que o perfil foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3d576-150">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="3d576-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3d576-151">roleScopeTagIds</span></span>|<span data-ttu-id="3d576-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d576-152">String collection</span></span>|<span data-ttu-id="3d576-153">Lista de Marcas de Escopo para esta entidade de Atualização de Qualidade.</span><span class="sxs-lookup"><span data-stu-id="3d576-153">List of Scope Tags for this Quality Update entity.</span></span>|
|<span data-ttu-id="3d576-154">releaseDateDisplayName</span><span class="sxs-lookup"><span data-stu-id="3d576-154">releaseDateDisplayName</span></span>|<span data-ttu-id="3d576-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d576-155">String</span></span>|<span data-ttu-id="3d576-156">Data de lançamento amigável a ser exibida para um lançamento de Atualização de Qualidade</span><span class="sxs-lookup"><span data-stu-id="3d576-156">Friendly release date to display for a Quality Update release</span></span>|
|<span data-ttu-id="3d576-157">deployableContentDisplayName</span><span class="sxs-lookup"><span data-stu-id="3d576-157">deployableContentDisplayName</span></span>|<span data-ttu-id="3d576-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d576-158">String</span></span>|<span data-ttu-id="3d576-159">Nome de exibição amigável do conteúdo implantável do perfil de atualização de qualidade</span><span class="sxs-lookup"><span data-stu-id="3d576-159">Friendly display name of the quality update profile deployable content</span></span>|



## <a name="response"></a><span data-ttu-id="3d576-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d576-160">Response</span></span>
<span data-ttu-id="3d576-161">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d576-161">If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d576-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d576-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d576-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d576-163">Request</span></span>
<span data-ttu-id="3d576-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d576-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}
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

### <a name="response"></a><span data-ttu-id="3d576-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d576-165">Response</span></span>
<span data-ttu-id="3d576-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d576-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




