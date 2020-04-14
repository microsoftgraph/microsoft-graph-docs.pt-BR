---
title: Criar windowsFeatureUpdateProfile
description: Criar um novo objeto windowsFeatureUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4fd5beb23e4581be24f6e119dae26403a245638c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471262"
---
# <a name="create-windowsfeatureupdateprofile"></a><span data-ttu-id="05281-103">Criar windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="05281-103">Create windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="05281-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05281-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05281-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="05281-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05281-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05281-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05281-107">Criar um novo objeto [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="05281-107">Create a new [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05281-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05281-108">Prerequisites</span></span>
<span data-ttu-id="05281-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05281-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05281-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05281-111">Permission type</span></span>|<span data-ttu-id="05281-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05281-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05281-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05281-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05281-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05281-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05281-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05281-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05281-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05281-116">Not supported.</span></span>|
|<span data-ttu-id="05281-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05281-117">Application</span></span>|<span data-ttu-id="05281-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05281-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05281-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05281-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles
```

## <a name="request-headers"></a><span data-ttu-id="05281-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05281-120">Request headers</span></span>
|<span data-ttu-id="05281-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05281-121">Header</span></span>|<span data-ttu-id="05281-122">Valor</span><span class="sxs-lookup"><span data-stu-id="05281-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05281-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="05281-123">Authorization</span></span>|<span data-ttu-id="05281-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05281-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05281-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05281-125">Accept</span></span>|<span data-ttu-id="05281-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05281-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05281-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05281-127">Request body</span></span>
<span data-ttu-id="05281-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsFeatureUpdateProfile.</span><span class="sxs-lookup"><span data-stu-id="05281-128">In the request body, supply a JSON representation for the windowsFeatureUpdateProfile object.</span></span>

<span data-ttu-id="05281-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsFeatureUpdateProfile.</span><span class="sxs-lookup"><span data-stu-id="05281-129">The following table shows the properties that are required when you create the windowsFeatureUpdateProfile.</span></span>

|<span data-ttu-id="05281-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05281-130">Property</span></span>|<span data-ttu-id="05281-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="05281-131">Type</span></span>|<span data-ttu-id="05281-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="05281-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05281-133">id</span><span class="sxs-lookup"><span data-stu-id="05281-133">id</span></span>|<span data-ttu-id="05281-134">String</span><span class="sxs-lookup"><span data-stu-id="05281-134">String</span></span>|<span data-ttu-id="05281-135">O identificador da entidade.</span><span class="sxs-lookup"><span data-stu-id="05281-135">The Identifier of the entity.</span></span>|
|<span data-ttu-id="05281-136">displayName</span><span class="sxs-lookup"><span data-stu-id="05281-136">displayName</span></span>|<span data-ttu-id="05281-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05281-137">String</span></span>|<span data-ttu-id="05281-138">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="05281-138">The display name of the profile.</span></span>|
|<span data-ttu-id="05281-139">description</span><span class="sxs-lookup"><span data-stu-id="05281-139">description</span></span>|<span data-ttu-id="05281-140">String</span><span class="sxs-lookup"><span data-stu-id="05281-140">String</span></span>|<span data-ttu-id="05281-141">A descrição do perfil especificado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="05281-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="05281-142">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="05281-142">featureUpdateVersion</span></span>|<span data-ttu-id="05281-143">String</span><span class="sxs-lookup"><span data-stu-id="05281-143">String</span></span>|<span data-ttu-id="05281-144">A versão de atualização de recurso que será implantada nos dispositivos direcionados por esse perfil.</span><span class="sxs-lookup"><span data-stu-id="05281-144">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="05281-145">A versão pode ser qualquer versão suportada por exemplo, 1709, 1803 ou 1809 e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="05281-145">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="05281-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05281-146">createdDateTime</span></span>|<span data-ttu-id="05281-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05281-147">DateTimeOffset</span></span>|<span data-ttu-id="05281-148">A data e hora em que o perfil foi criado.</span><span class="sxs-lookup"><span data-stu-id="05281-148">The date time that the profile was created.</span></span>|
|<span data-ttu-id="05281-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05281-149">lastModifiedDateTime</span></span>|<span data-ttu-id="05281-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05281-150">DateTimeOffset</span></span>|<span data-ttu-id="05281-151">A data e hora em que o perfil foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="05281-151">The date time that the profile was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="05281-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="05281-152">Response</span></span>
<span data-ttu-id="05281-153">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05281-153">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05281-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05281-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="05281-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05281-155">Request</span></span>
<span data-ttu-id="05281-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05281-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles
Content-type: application/json
Content-length: 207

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value"
}
```

### <a name="response"></a><span data-ttu-id="05281-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="05281-157">Response</span></span>
<span data-ttu-id="05281-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05281-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



