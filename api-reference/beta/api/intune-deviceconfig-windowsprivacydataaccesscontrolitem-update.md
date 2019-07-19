---
title: Atualizar windowsPrivacyDataAccessControlItem
description: Atualiza as propriedades de um objeto windowsPrivacyDataAccessControlItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3208d5f4eb7ac1fe20ea3d280f8522358ba8867
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961375"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="59be0-103">Atualizar windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="59be0-103">Update windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="59be0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59be0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59be0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59be0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59be0-106">Atualiza as propriedades de um objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="59be0-106">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59be0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59be0-107">Prerequisites</span></span>
<span data-ttu-id="59be0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59be0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59be0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59be0-110">Permission type</span></span>|<span data-ttu-id="59be0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59be0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59be0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59be0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59be0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59be0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="59be0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59be0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59be0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59be0-115">Not supported.</span></span>|
|<span data-ttu-id="59be0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59be0-116">Application</span></span>|<span data-ttu-id="59be0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59be0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59be0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59be0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="59be0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59be0-119">Request headers</span></span>
|<span data-ttu-id="59be0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59be0-120">Header</span></span>|<span data-ttu-id="59be0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="59be0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59be0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="59be0-122">Authorization</span></span>|<span data-ttu-id="59be0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59be0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59be0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="59be0-124">Accept</span></span>|<span data-ttu-id="59be0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59be0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59be0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59be0-126">Request body</span></span>
<span data-ttu-id="59be0-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="59be0-127">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="59be0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span><span class="sxs-lookup"><span data-stu-id="59be0-128">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="59be0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59be0-129">Property</span></span>|<span data-ttu-id="59be0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="59be0-130">Type</span></span>|<span data-ttu-id="59be0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="59be0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59be0-132">id</span><span class="sxs-lookup"><span data-stu-id="59be0-132">id</span></span>|<span data-ttu-id="59be0-133">String</span><span class="sxs-lookup"><span data-stu-id="59be0-133">String</span></span>|<span data-ttu-id="59be0-134">A chave de WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="59be0-134">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="59be0-135">accessLevel</span><span class="sxs-lookup"><span data-stu-id="59be0-135">accessLevel</span></span>|[<span data-ttu-id="59be0-136">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="59be0-136">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="59be0-137">Isso indica um nível de acesso para a categoria de dados de privacidade à qual o aplicativo especificado será atribuído.</span><span class="sxs-lookup"><span data-stu-id="59be0-137">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="59be0-138">Os valores possíveis são: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="59be0-138">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="59be0-139">dataCategory</span><span class="sxs-lookup"><span data-stu-id="59be0-139">dataCategory</span></span>|[<span data-ttu-id="59be0-140">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="59be0-140">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="59be0-141">Isso indica uma categoria de dados de privacidade à qual o controle de acesso específico será aplicado.</span><span class="sxs-lookup"><span data-stu-id="59be0-141">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="59be0-142">Os valores possíveis são `notConfigured`: `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location` `messaging` `microphone`,,, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices` ,,,,,,,, .</span><span class="sxs-lookup"><span data-stu-id="59be0-142">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="59be0-143">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="59be0-143">appPackageFamilyName</span></span>|<span data-ttu-id="59be0-144">String</span><span class="sxs-lookup"><span data-stu-id="59be0-144">String</span></span>|<span data-ttu-id="59be0-145">O nome da família de pacote de um aplicativo Windows.</span><span class="sxs-lookup"><span data-stu-id="59be0-145">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="59be0-146">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="59be0-146">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="59be0-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="59be0-147">appDisplayName</span></span>|<span data-ttu-id="59be0-148">String</span><span class="sxs-lookup"><span data-stu-id="59be0-148">String</span></span>|<span data-ttu-id="59be0-149">O nome da família de pacote de um aplicativo Windows.</span><span class="sxs-lookup"><span data-stu-id="59be0-149">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="59be0-150">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="59be0-150">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="59be0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="59be0-151">Response</span></span>
<span data-ttu-id="59be0-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59be0-152">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59be0-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59be0-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="59be0-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59be0-154">Request</span></span>
<span data-ttu-id="59be0-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59be0-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
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

### <a name="response"></a><span data-ttu-id="59be0-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="59be0-156">Response</span></span>
<span data-ttu-id="59be0-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59be0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





