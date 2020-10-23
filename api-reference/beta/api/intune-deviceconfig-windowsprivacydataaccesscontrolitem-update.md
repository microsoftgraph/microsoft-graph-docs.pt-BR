---
title: Atualizar windowsPrivacyDataAccessControlItem
description: Atualiza as propriedades de um objeto windowsPrivacyDataAccessControlItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ff939d30ef615ea85507460ca9dd48a19446363
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693336"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="9bba9-103">Atualizar windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="9bba9-103">Update windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="9bba9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bba9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bba9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9bba9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bba9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9bba9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bba9-107">Atualiza as propriedades de um objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="9bba9-107">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bba9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9bba9-108">Prerequisites</span></span>
<span data-ttu-id="9bba9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bba9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bba9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bba9-111">Permission type</span></span>|<span data-ttu-id="9bba9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9bba9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bba9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bba9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bba9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bba9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9bba9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bba9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bba9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bba9-116">Not supported.</span></span>|
|<span data-ttu-id="9bba9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bba9-117">Application</span></span>|<span data-ttu-id="9bba9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bba9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bba9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bba9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="9bba9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bba9-120">Request headers</span></span>
|<span data-ttu-id="9bba9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bba9-121">Header</span></span>|<span data-ttu-id="9bba9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9bba9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bba9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bba9-123">Authorization</span></span>|<span data-ttu-id="9bba9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bba9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bba9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9bba9-125">Accept</span></span>|<span data-ttu-id="9bba9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bba9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bba9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bba9-127">Request body</span></span>
<span data-ttu-id="9bba9-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="9bba9-128">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="9bba9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span><span class="sxs-lookup"><span data-stu-id="9bba9-129">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="9bba9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bba9-130">Property</span></span>|<span data-ttu-id="9bba9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bba9-131">Type</span></span>|<span data-ttu-id="9bba9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bba9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bba9-133">id</span><span class="sxs-lookup"><span data-stu-id="9bba9-133">id</span></span>|<span data-ttu-id="9bba9-134">String</span><span class="sxs-lookup"><span data-stu-id="9bba9-134">String</span></span>|<span data-ttu-id="9bba9-135">A chave de WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="9bba9-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="9bba9-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="9bba9-136">accessLevel</span></span>|[<span data-ttu-id="9bba9-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="9bba9-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="9bba9-138">Isso indica um nível de acesso para a categoria de dados de privacidade à qual o aplicativo especificado será atribuído.</span><span class="sxs-lookup"><span data-stu-id="9bba9-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="9bba9-139">Os valores possíveis são: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="9bba9-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="9bba9-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="9bba9-140">dataCategory</span></span>|[<span data-ttu-id="9bba9-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="9bba9-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="9bba9-142">Isso indica uma categoria de dados de privacidade à qual o controle de acesso específico será aplicado.</span><span class="sxs-lookup"><span data-stu-id="9bba9-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="9bba9-143">Os valores possíveis são:, `notConfigured` `accountInfo` ,,,,,,,,,,,,,, `appsRunInBackground` `calendar` ,,,,,, `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone` `motion` , `notifications` , `phone` , `radios` , `tasks` , `syncWithDevices` , `trustedDevices` .</span><span class="sxs-lookup"><span data-stu-id="9bba9-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="9bba9-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="9bba9-144">appPackageFamilyName</span></span>|<span data-ttu-id="9bba9-145">String</span><span class="sxs-lookup"><span data-stu-id="9bba9-145">String</span></span>|<span data-ttu-id="9bba9-146">O nome da família de pacote de um aplicativo Windows.</span><span class="sxs-lookup"><span data-stu-id="9bba9-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="9bba9-147">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="9bba9-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="9bba9-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="9bba9-148">appDisplayName</span></span>|<span data-ttu-id="9bba9-149">String</span><span class="sxs-lookup"><span data-stu-id="9bba9-149">String</span></span>|<span data-ttu-id="9bba9-150">O nome da família de pacote de um aplicativo Windows.</span><span class="sxs-lookup"><span data-stu-id="9bba9-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="9bba9-151">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="9bba9-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="9bba9-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bba9-152">Response</span></span>
<span data-ttu-id="9bba9-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bba9-153">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bba9-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bba9-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bba9-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bba9-155">Request</span></span>
<span data-ttu-id="9bba9-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bba9-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9bba9-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bba9-157">Response</span></span>
<span data-ttu-id="9bba9-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bba9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





