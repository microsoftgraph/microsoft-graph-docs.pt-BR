---
title: Criar windowsPrivacyDataAccessControlItem
description: Criar um novo objeto windowsPrivacyDataAccessControlItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91a9ed35325ec9d85ead030d07ddef973cbde0d0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42473952"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="1838b-103">Criar windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="1838b-103">Create windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="1838b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1838b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1838b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1838b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1838b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1838b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1838b-107">Criar um novo objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="1838b-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1838b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1838b-108">Prerequisites</span></span>
<span data-ttu-id="1838b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1838b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1838b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1838b-111">Permission type</span></span>|<span data-ttu-id="1838b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1838b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1838b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1838b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1838b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1838b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1838b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1838b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1838b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1838b-116">Not supported.</span></span>|
|<span data-ttu-id="1838b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1838b-117">Application</span></span>|<span data-ttu-id="1838b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1838b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1838b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1838b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="1838b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1838b-120">Request headers</span></span>
|<span data-ttu-id="1838b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1838b-121">Header</span></span>|<span data-ttu-id="1838b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1838b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1838b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1838b-123">Authorization</span></span>|<span data-ttu-id="1838b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1838b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1838b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1838b-125">Accept</span></span>|<span data-ttu-id="1838b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1838b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1838b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1838b-127">Request body</span></span>
<span data-ttu-id="1838b-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="1838b-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="1838b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="1838b-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="1838b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1838b-130">Property</span></span>|<span data-ttu-id="1838b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1838b-131">Type</span></span>|<span data-ttu-id="1838b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1838b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1838b-133">id</span><span class="sxs-lookup"><span data-stu-id="1838b-133">id</span></span>|<span data-ttu-id="1838b-134">String</span><span class="sxs-lookup"><span data-stu-id="1838b-134">String</span></span>|<span data-ttu-id="1838b-135">A chave de WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="1838b-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="1838b-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="1838b-136">accessLevel</span></span>|[<span data-ttu-id="1838b-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="1838b-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="1838b-138">Isso indica um nível de acesso para a categoria de dados de privacidade à qual o aplicativo especificado será atribuído.</span><span class="sxs-lookup"><span data-stu-id="1838b-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="1838b-139">Os valores possíveis são: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="1838b-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="1838b-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="1838b-140">dataCategory</span></span>|[<span data-ttu-id="1838b-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="1838b-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="1838b-142">Isso indica uma categoria de dados de privacidade à qual o controle de acesso específico será aplicado.</span><span class="sxs-lookup"><span data-stu-id="1838b-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="1838b-143">Os valores possíveis são `notConfigured`: `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="1838b-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="1838b-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="1838b-144">appPackageFamilyName</span></span>|<span data-ttu-id="1838b-145">String</span><span class="sxs-lookup"><span data-stu-id="1838b-145">String</span></span>|<span data-ttu-id="1838b-146">O nome da família de pacote de um aplicativo Windows.</span><span class="sxs-lookup"><span data-stu-id="1838b-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="1838b-147">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="1838b-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="1838b-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="1838b-148">appDisplayName</span></span>|<span data-ttu-id="1838b-149">String</span><span class="sxs-lookup"><span data-stu-id="1838b-149">String</span></span>|<span data-ttu-id="1838b-150">O nome da família de pacote de um aplicativo Windows.</span><span class="sxs-lookup"><span data-stu-id="1838b-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="1838b-151">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="1838b-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="1838b-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="1838b-152">Response</span></span>
<span data-ttu-id="1838b-153">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1838b-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1838b-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1838b-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="1838b-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1838b-155">Request</span></span>
<span data-ttu-id="1838b-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1838b-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1838b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="1838b-157">Response</span></span>
<span data-ttu-id="1838b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1838b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





