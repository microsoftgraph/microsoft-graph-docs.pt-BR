---
title: Criar windowsPrivacyDataAccessControlItem
description: Criar um novo objeto windowsPrivacyDataAccessControlItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5642147fd8299fc7f798b7d771bdd72779da39b6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181452"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="ae107-103">Criar windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="ae107-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="ae107-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae107-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae107-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae107-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae107-106">Criar um novo objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="ae107-106">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae107-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae107-107">Prerequisites</span></span>
<span data-ttu-id="ae107-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae107-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae107-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae107-110">Permission type</span></span>|<span data-ttu-id="ae107-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae107-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae107-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae107-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae107-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae107-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae107-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae107-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae107-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae107-115">Not supported.</span></span>|
|<span data-ttu-id="ae107-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae107-116">Application</span></span>|<span data-ttu-id="ae107-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae107-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae107-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae107-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="ae107-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae107-119">Request headers</span></span>
|<span data-ttu-id="ae107-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae107-120">Header</span></span>|<span data-ttu-id="ae107-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ae107-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae107-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae107-122">Authorization</span></span>|<span data-ttu-id="ae107-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae107-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae107-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae107-124">Accept</span></span>|<span data-ttu-id="ae107-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae107-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae107-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae107-126">Request body</span></span>
<span data-ttu-id="ae107-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="ae107-127">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="ae107-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="ae107-128">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="ae107-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae107-129">Property</span></span>|<span data-ttu-id="ae107-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae107-130">Type</span></span>|<span data-ttu-id="ae107-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae107-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae107-132">id</span><span class="sxs-lookup"><span data-stu-id="ae107-132">id</span></span>|<span data-ttu-id="ae107-133">String</span><span class="sxs-lookup"><span data-stu-id="ae107-133">String</span></span>|<span data-ttu-id="ae107-134">A chave de WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="ae107-134">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="ae107-135">accessLevel</span><span class="sxs-lookup"><span data-stu-id="ae107-135">accessLevel</span></span>|[<span data-ttu-id="ae107-136">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="ae107-136">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="ae107-137">Isso indica um nível de acesso para a categoria de dados de privacidade à qual o aplicativo especificado será atribuído.</span><span class="sxs-lookup"><span data-stu-id="ae107-137">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="ae107-138">Os valores possíveis são: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="ae107-138">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="ae107-139">dataCategory</span><span class="sxs-lookup"><span data-stu-id="ae107-139">dataCategory</span></span>|[<span data-ttu-id="ae107-140">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="ae107-140">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="ae107-141">Isso indica uma categoria de dados de privacidade à qual o controle de acesso específico será aplicado.</span><span class="sxs-lookup"><span data-stu-id="ae107-141">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="ae107-142">Os valores possíveis são `notConfigured`: `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location` `messaging` `microphone`,,, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices` ,,,,,,,, .</span><span class="sxs-lookup"><span data-stu-id="ae107-142">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="ae107-143">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="ae107-143">appPackageFamilyName</span></span>|<span data-ttu-id="ae107-144">String</span><span class="sxs-lookup"><span data-stu-id="ae107-144">String</span></span>|<span data-ttu-id="ae107-145">O nome da família de pacote de um aplicativo Windows.</span><span class="sxs-lookup"><span data-stu-id="ae107-145">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="ae107-146">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="ae107-146">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="ae107-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="ae107-147">appDisplayName</span></span>|<span data-ttu-id="ae107-148">String</span><span class="sxs-lookup"><span data-stu-id="ae107-148">String</span></span>|<span data-ttu-id="ae107-149">O nome da família de pacote de um aplicativo Windows.</span><span class="sxs-lookup"><span data-stu-id="ae107-149">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="ae107-150">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="ae107-150">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="ae107-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae107-151">Response</span></span>
<span data-ttu-id="ae107-152">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae107-152">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae107-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae107-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae107-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae107-154">Request</span></span>
<span data-ttu-id="ae107-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae107-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ae107-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae107-156">Response</span></span>
<span data-ttu-id="ae107-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae107-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




