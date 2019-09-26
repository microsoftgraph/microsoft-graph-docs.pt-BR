---
title: Atualizar windowsFeatureUpdateProfile
description: Atualiza as propriedades de um objeto windowsFeatureUpdateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 527be763c4fe00468fce075ffd139125668797ec
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199502"
---
# <a name="update-windowsfeatureupdateprofile"></a><span data-ttu-id="38ff6-103">Atualizar windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="38ff6-103">Update windowsFeatureUpdateProfile</span></span>

> <span data-ttu-id="38ff6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="38ff6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38ff6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38ff6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38ff6-106">Atualiza as propriedades de um objeto [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="38ff6-106">Update the properties of a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38ff6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38ff6-107">Prerequisites</span></span>
<span data-ttu-id="38ff6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38ff6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38ff6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38ff6-110">Permission type</span></span>|<span data-ttu-id="38ff6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38ff6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38ff6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38ff6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38ff6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38ff6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38ff6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38ff6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38ff6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38ff6-115">Not supported.</span></span>|
|<span data-ttu-id="38ff6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38ff6-116">Application</span></span>|<span data-ttu-id="38ff6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38ff6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38ff6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38ff6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="38ff6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38ff6-119">Request headers</span></span>
|<span data-ttu-id="38ff6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38ff6-120">Header</span></span>|<span data-ttu-id="38ff6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="38ff6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38ff6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="38ff6-122">Authorization</span></span>|<span data-ttu-id="38ff6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38ff6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38ff6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38ff6-124">Accept</span></span>|<span data-ttu-id="38ff6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38ff6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38ff6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38ff6-126">Request body</span></span>
<span data-ttu-id="38ff6-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="38ff6-127">In the request body, supply a JSON representation for the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

<span data-ttu-id="38ff6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="38ff6-128">The following table shows the properties that are required when you create the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span></span>

|<span data-ttu-id="38ff6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38ff6-129">Property</span></span>|<span data-ttu-id="38ff6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="38ff6-130">Type</span></span>|<span data-ttu-id="38ff6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="38ff6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38ff6-132">id</span><span class="sxs-lookup"><span data-stu-id="38ff6-132">id</span></span>|<span data-ttu-id="38ff6-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38ff6-133">String</span></span>|<span data-ttu-id="38ff6-134">O identificador da entidade.</span><span class="sxs-lookup"><span data-stu-id="38ff6-134">The Identifier of the entity.</span></span>|
|<span data-ttu-id="38ff6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="38ff6-135">displayName</span></span>|<span data-ttu-id="38ff6-136">String</span><span class="sxs-lookup"><span data-stu-id="38ff6-136">String</span></span>|<span data-ttu-id="38ff6-137">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="38ff6-137">The display name of the profile.</span></span>|
|<span data-ttu-id="38ff6-138">descrição</span><span class="sxs-lookup"><span data-stu-id="38ff6-138">description</span></span>|<span data-ttu-id="38ff6-139">String</span><span class="sxs-lookup"><span data-stu-id="38ff6-139">String</span></span>|<span data-ttu-id="38ff6-140">A descrição do perfil especificado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="38ff6-140">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="38ff6-141">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="38ff6-141">featureUpdateVersion</span></span>|<span data-ttu-id="38ff6-142">String</span><span class="sxs-lookup"><span data-stu-id="38ff6-142">String</span></span>|<span data-ttu-id="38ff6-143">A versão de atualização de recurso que será implantada nos dispositivos direcionados por esse perfil.</span><span class="sxs-lookup"><span data-stu-id="38ff6-143">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="38ff6-144">A versão pode ser qualquer versão suportada por exemplo, 1709, 1803 ou 1809 e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="38ff6-144">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="38ff6-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38ff6-145">createdDateTime</span></span>|<span data-ttu-id="38ff6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38ff6-146">DateTimeOffset</span></span>|<span data-ttu-id="38ff6-147">A data e hora em que o perfil foi criado.</span><span class="sxs-lookup"><span data-stu-id="38ff6-147">The date time that the profile was created.</span></span>|
|<span data-ttu-id="38ff6-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38ff6-148">lastModifiedDateTime</span></span>|<span data-ttu-id="38ff6-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38ff6-149">DateTimeOffset</span></span>|<span data-ttu-id="38ff6-150">A data e hora em que o perfil foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="38ff6-150">The date time that the profile was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="38ff6-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="38ff6-151">Response</span></span>
<span data-ttu-id="38ff6-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38ff6-152">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38ff6-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38ff6-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="38ff6-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38ff6-154">Request</span></span>
<span data-ttu-id="38ff6-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38ff6-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
Content-type: application/json
Content-length: 207

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value"
}
```

### <a name="response"></a><span data-ttu-id="38ff6-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="38ff6-156">Response</span></span>
<span data-ttu-id="38ff6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38ff6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




