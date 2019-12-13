---
title: Atualizar windowsFeatureUpdateProfile
description: Atualiza as propriedades de um objeto windowsFeatureUpdateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06272e3ddc3c92c2f042e08b010cbc8197cb49b5
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939266"
---
# <a name="update-windowsfeatureupdateprofile"></a><span data-ttu-id="0c987-103">Atualizar windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="0c987-103">Update windowsFeatureUpdateProfile</span></span>

> <span data-ttu-id="0c987-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c987-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c987-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c987-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c987-106">Atualiza as propriedades de um objeto [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0c987-106">Update the properties of a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c987-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c987-107">Prerequisites</span></span>
<span data-ttu-id="0c987-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c987-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c987-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c987-110">Permission type</span></span>|<span data-ttu-id="0c987-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c987-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c987-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c987-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c987-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c987-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c987-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c987-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c987-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c987-115">Not supported.</span></span>|
|<span data-ttu-id="0c987-116">Application</span><span class="sxs-lookup"><span data-stu-id="0c987-116">Application</span></span>|<span data-ttu-id="0c987-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c987-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c987-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c987-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="0c987-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c987-119">Request headers</span></span>
|<span data-ttu-id="0c987-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c987-120">Header</span></span>|<span data-ttu-id="0c987-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0c987-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c987-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c987-122">Authorization</span></span>|<span data-ttu-id="0c987-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c987-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c987-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c987-124">Accept</span></span>|<span data-ttu-id="0c987-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c987-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c987-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c987-126">Request body</span></span>
<span data-ttu-id="0c987-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0c987-127">In the request body, supply a JSON representation for the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

<span data-ttu-id="0c987-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0c987-128">The following table shows the properties that are required when you create the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span></span>

|<span data-ttu-id="0c987-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c987-129">Property</span></span>|<span data-ttu-id="0c987-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c987-130">Type</span></span>|<span data-ttu-id="0c987-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c987-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c987-132">id</span><span class="sxs-lookup"><span data-stu-id="0c987-132">id</span></span>|<span data-ttu-id="0c987-133">String</span><span class="sxs-lookup"><span data-stu-id="0c987-133">String</span></span>|<span data-ttu-id="0c987-134">O identificador da entidade.</span><span class="sxs-lookup"><span data-stu-id="0c987-134">The Identifier of the entity.</span></span>|
|<span data-ttu-id="0c987-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0c987-135">displayName</span></span>|<span data-ttu-id="0c987-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c987-136">String</span></span>|<span data-ttu-id="0c987-137">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="0c987-137">The display name of the profile.</span></span>|
|<span data-ttu-id="0c987-138">description</span><span class="sxs-lookup"><span data-stu-id="0c987-138">description</span></span>|<span data-ttu-id="0c987-139">String</span><span class="sxs-lookup"><span data-stu-id="0c987-139">String</span></span>|<span data-ttu-id="0c987-140">A descrição do perfil especificado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="0c987-140">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="0c987-141">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="0c987-141">featureUpdateVersion</span></span>|<span data-ttu-id="0c987-142">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0c987-142">String</span></span>|<span data-ttu-id="0c987-143">A versão de atualização de recurso que será implantada nos dispositivos direcionados por esse perfil.</span><span class="sxs-lookup"><span data-stu-id="0c987-143">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="0c987-144">A versão pode ser qualquer versão suportada por exemplo, 1709, 1803 ou 1809 e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="0c987-144">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="0c987-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c987-145">createdDateTime</span></span>|<span data-ttu-id="0c987-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c987-146">DateTimeOffset</span></span>|<span data-ttu-id="0c987-147">A data e hora em que o perfil foi criado.</span><span class="sxs-lookup"><span data-stu-id="0c987-147">The date time that the profile was created.</span></span>|
|<span data-ttu-id="0c987-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c987-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0c987-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c987-149">DateTimeOffset</span></span>|<span data-ttu-id="0c987-150">A data e hora em que o perfil foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0c987-150">The date time that the profile was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="0c987-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c987-151">Response</span></span>
<span data-ttu-id="0c987-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c987-152">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c987-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c987-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c987-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c987-154">Request</span></span>
<span data-ttu-id="0c987-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c987-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c987-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c987-156">Response</span></span>
<span data-ttu-id="0c987-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c987-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





