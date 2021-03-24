---
title: Atualizar windowsPrivacyDataAccessControlItem
description: Atualize as propriedades de um objeto windowsPrivacyDataAccessControlItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 85c912c244d2554fd9a05ccaedf16bf60cfc565d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147081"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="0ea3f-103">Atualizar windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="0ea3f-103">Update windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="0ea3f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ea3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ea3f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ea3f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ea3f-107">Atualize as propriedades de um [objeto windowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ea3f-107">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ea3f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ea3f-108">Prerequisites</span></span>
<span data-ttu-id="0ea3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ea3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea3f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ea3f-111">Permission type</span></span>|<span data-ttu-id="0ea3f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ea3f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ea3f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ea3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ea3f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea3f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ea3f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ea3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ea3f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-116">Not supported.</span></span>|
|<span data-ttu-id="0ea3f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ea3f-117">Application</span></span>|<span data-ttu-id="0ea3f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea3f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ea3f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ea3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="0ea3f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ea3f-120">Request headers</span></span>
|<span data-ttu-id="0ea3f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ea3f-121">Header</span></span>|<span data-ttu-id="0ea3f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0ea3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ea3f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ea3f-123">Authorization</span></span>|<span data-ttu-id="0ea3f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ea3f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0ea3f-125">Accept</span></span>|<span data-ttu-id="0ea3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ea3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ea3f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ea3f-127">Request body</span></span>
<span data-ttu-id="0ea3f-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ea3f-128">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="0ea3f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span><span class="sxs-lookup"><span data-stu-id="0ea3f-129">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="0ea3f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ea3f-130">Property</span></span>|<span data-ttu-id="0ea3f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ea3f-131">Type</span></span>|<span data-ttu-id="0ea3f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ea3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ea3f-133">id</span><span class="sxs-lookup"><span data-stu-id="0ea3f-133">id</span></span>|<span data-ttu-id="0ea3f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ea3f-134">String</span></span>|<span data-ttu-id="0ea3f-135">A chave do WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="0ea3f-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="0ea3f-136">accessLevel</span></span>|[<span data-ttu-id="0ea3f-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="0ea3f-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="0ea3f-138">Isso indica um nível de acesso para a categoria de dados de privacidade ao qual o aplicativo especificado será dado.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="0ea3f-139">Os valores possíveis são: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="0ea3f-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="0ea3f-140">dataCategory</span></span>|[<span data-ttu-id="0ea3f-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="0ea3f-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="0ea3f-142">Isso indica uma categoria de dados de privacidade à qual o controle de acesso específico será aplicado.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="0ea3f-143">Os valores possíveis são: `notConfigured` , , , , , , , , , `accountInfo` , , , , `appsRunInBackground` , , , `calendar` , `callHistory` `camera` , `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone` `motion` `notifications` `phone` `radios` `tasks` . `syncWithDevices` `trustedDevices`</span><span class="sxs-lookup"><span data-stu-id="0ea3f-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="0ea3f-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="0ea3f-144">appPackageFamilyName</span></span>|<span data-ttu-id="0ea3f-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ea3f-145">String</span></span>|<span data-ttu-id="0ea3f-146">O Nome da Família de Pacotes de um aplicativo do Windows.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="0ea3f-147">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="0ea3f-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="0ea3f-148">appDisplayName</span></span>|<span data-ttu-id="0ea3f-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ea3f-149">String</span></span>|<span data-ttu-id="0ea3f-150">O Nome da Família de Pacotes de um aplicativo do Windows.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="0ea3f-151">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="0ea3f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ea3f-152">Response</span></span>
<span data-ttu-id="0ea3f-153">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-153">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ea3f-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ea3f-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ea3f-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ea3f-155">Request</span></span>
<span data-ttu-id="0ea3f-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ea3f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ea3f-157">Response</span></span>
<span data-ttu-id="0ea3f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ea3f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




