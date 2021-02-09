---
title: Atualizar windowsQualityUpdateProfile
description: Atualizar as propriedades de um objeto windowsQualityUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1733570906276f259f2f8fa4147df9b61e390a23
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160114"
---
# <a name="update-windowsqualityupdateprofile"></a><span data-ttu-id="6fa6f-103">Atualizar windowsQualityUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="6fa6f-103">Update windowsQualityUpdateProfile</span></span>

<span data-ttu-id="6fa6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fa6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fa6f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fa6f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fa6f-107">Atualizar as propriedades de um [objeto windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6fa6f-107">Update the properties of a [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fa6f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6fa6f-108">Prerequisites</span></span>
<span data-ttu-id="6fa6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fa6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fa6f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fa6f-111">Permission type</span></span>|<span data-ttu-id="6fa6f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6fa6f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fa6f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fa6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fa6f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa6f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6fa6f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fa6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fa6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-116">Not supported.</span></span>|
|<span data-ttu-id="6fa6f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fa6f-117">Application</span></span>|<span data-ttu-id="6fa6f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa6f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fa6f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fa6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="6fa6f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fa6f-120">Request headers</span></span>
|<span data-ttu-id="6fa6f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6fa6f-121">Header</span></span>|<span data-ttu-id="6fa6f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6fa6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fa6f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fa6f-123">Authorization</span></span>|<span data-ttu-id="6fa6f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fa6f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6fa6f-125">Accept</span></span>|<span data-ttu-id="6fa6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fa6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fa6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fa6f-127">Request body</span></span>
<span data-ttu-id="6fa6f-128">No corpo da solicitação, fornece uma representação JSON do [objeto windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6fa6f-128">In the request body, supply a JSON representation for the [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object.</span></span>

<span data-ttu-id="6fa6f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6fa6f-129">The following table shows the properties that are required when you create the [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md).</span></span>

|<span data-ttu-id="6fa6f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fa6f-130">Property</span></span>|<span data-ttu-id="6fa6f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fa6f-131">Type</span></span>|<span data-ttu-id="6fa6f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fa6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fa6f-133">id</span><span class="sxs-lookup"><span data-stu-id="6fa6f-133">id</span></span>|<span data-ttu-id="6fa6f-134">String</span><span class="sxs-lookup"><span data-stu-id="6fa6f-134">String</span></span>|<span data-ttu-id="6fa6f-135">A ID de política do Intune.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-135">The Intune policy id.</span></span>|
|<span data-ttu-id="6fa6f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6fa6f-136">displayName</span></span>|<span data-ttu-id="6fa6f-137">String</span><span class="sxs-lookup"><span data-stu-id="6fa6f-137">String</span></span>|<span data-ttu-id="6fa6f-138">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-138">The display name for the profile.</span></span>|
|<span data-ttu-id="6fa6f-139">description</span><span class="sxs-lookup"><span data-stu-id="6fa6f-139">description</span></span>|<span data-ttu-id="6fa6f-140">String</span><span class="sxs-lookup"><span data-stu-id="6fa6f-140">String</span></span>|<span data-ttu-id="6fa6f-141">A descrição do perfil especificado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="6fa6f-142">expeditedUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="6fa6f-142">expeditedUpdateSettings</span></span>|[<span data-ttu-id="6fa6f-143">expeditedWindowsQualityUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="6fa6f-143">expeditedWindowsQualityUpdateSettings</span></span>](../resources/intune-softwareupdate-expeditedwindowsqualityupdatesettings.md)|<span data-ttu-id="6fa6f-144">Configurações de atualização agilizadas.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-144">Expedited update settings.</span></span>|
|<span data-ttu-id="6fa6f-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fa6f-145">createdDateTime</span></span>|<span data-ttu-id="6fa6f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fa6f-146">DateTimeOffset</span></span>|<span data-ttu-id="6fa6f-147">A data e a hora em que o perfil foi criado.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-147">The date time that the profile was created.</span></span>|
|<span data-ttu-id="6fa6f-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fa6f-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6fa6f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fa6f-149">DateTimeOffset</span></span>|<span data-ttu-id="6fa6f-150">A data em que o perfil foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-150">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="6fa6f-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6fa6f-151">roleScopeTagIds</span></span>|<span data-ttu-id="6fa6f-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6fa6f-152">String collection</span></span>|<span data-ttu-id="6fa6f-153">Lista de Marcas de Escopo para esta entidade de Atualização de Qualidade.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-153">List of Scope Tags for this Quality Update entity.</span></span>|



## <a name="response"></a><span data-ttu-id="6fa6f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fa6f-154">Response</span></span>
<span data-ttu-id="6fa6f-155">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-155">If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fa6f-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fa6f-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fa6f-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fa6f-157">Request</span></span>
<span data-ttu-id="6fa6f-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}
Content-type: application/json
Content-length: 418

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="6fa6f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fa6f-159">Response</span></span>
<span data-ttu-id="6fa6f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fa6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

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
  ]
}
```




