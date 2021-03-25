---
title: Criar windowsPrivacyDataAccessControlItem
description: Crie um novo objeto windowsPrivacyDataAccessControlItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01b052e50bede136d1c4cf3f8ea2b555ff5fae48
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154704"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="a3a5a-103">Criar windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="a3a5a-103">Create windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="a3a5a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3a5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3a5a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3a5a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3a5a-107">Crie um novo [objeto windowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="a3a5a-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3a5a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3a5a-108">Prerequisites</span></span>
<span data-ttu-id="a3a5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3a5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3a5a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3a5a-111">Permission type</span></span>|<span data-ttu-id="a3a5a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3a5a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3a5a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3a5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3a5a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3a5a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3a5a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3a5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3a5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-116">Not supported.</span></span>|
|<span data-ttu-id="a3a5a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3a5a-117">Application</span></span>|<span data-ttu-id="a3a5a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3a5a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3a5a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3a5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="a3a5a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3a5a-120">Request headers</span></span>
|<span data-ttu-id="a3a5a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3a5a-121">Header</span></span>|<span data-ttu-id="a3a5a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a3a5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3a5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3a5a-123">Authorization</span></span>|<span data-ttu-id="a3a5a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3a5a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a3a5a-125">Accept</span></span>|<span data-ttu-id="a3a5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3a5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3a5a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3a5a-127">Request body</span></span>
<span data-ttu-id="a3a5a-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="a3a5a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="a3a5a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3a5a-130">Property</span></span>|<span data-ttu-id="a3a5a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3a5a-131">Type</span></span>|<span data-ttu-id="a3a5a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3a5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3a5a-133">id</span><span class="sxs-lookup"><span data-stu-id="a3a5a-133">id</span></span>|<span data-ttu-id="a3a5a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3a5a-134">String</span></span>|<span data-ttu-id="a3a5a-135">A chave do WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="a3a5a-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="a3a5a-136">accessLevel</span></span>|[<span data-ttu-id="a3a5a-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="a3a5a-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="a3a5a-138">Isso indica um nível de acesso para a categoria de dados de privacidade ao qual o aplicativo especificado será dado.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="a3a5a-139">Os valores possíveis são: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="a3a5a-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="a3a5a-140">dataCategory</span></span>|[<span data-ttu-id="a3a5a-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="a3a5a-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="a3a5a-142">Isso indica uma categoria de dados de privacidade à qual o controle de acesso específico será aplicado.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="a3a5a-143">Os valores possíveis são: `notConfigured` , , , , , , , , , `accountInfo` , , , , `appsRunInBackground` , , , `calendar` , `callHistory` `camera` , `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone` `motion` `notifications` `phone` `radios` `tasks` . `syncWithDevices` `trustedDevices`</span><span class="sxs-lookup"><span data-stu-id="a3a5a-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="a3a5a-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="a3a5a-144">appPackageFamilyName</span></span>|<span data-ttu-id="a3a5a-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3a5a-145">String</span></span>|<span data-ttu-id="a3a5a-146">O Nome da Família de Pacotes de um aplicativo do Windows.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="a3a5a-147">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="a3a5a-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="a3a5a-148">appDisplayName</span></span>|<span data-ttu-id="a3a5a-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3a5a-149">String</span></span>|<span data-ttu-id="a3a5a-150">O Nome da Família de Pacotes de um aplicativo do Windows.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="a3a5a-151">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="a3a5a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3a5a-152">Response</span></span>
<span data-ttu-id="a3a5a-153">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3a5a-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3a5a-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3a5a-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3a5a-155">Request</span></span>
<span data-ttu-id="a3a5a-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="a3a5a-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3a5a-157">Response</span></span>
<span data-ttu-id="a3a5a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3a5a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 299

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "03b15556-5556-03b1-5655-b1035655b103",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```




