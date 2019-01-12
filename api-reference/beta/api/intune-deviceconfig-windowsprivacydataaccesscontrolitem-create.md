---
title: Criar windowsPrivacyDataAccessControlItem
description: Crie um novo objeto de windowsPrivacyDataAccessControlItem.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3ec9aa9f4b8351c4f64ce468027f1f46e7d139a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948930"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="13b7f-103">Criar windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="13b7f-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="13b7f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="13b7f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13b7f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="13b7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13b7f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="13b7f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13b7f-107">Crie um novo objeto de [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="13b7f-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="13b7f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13b7f-108">Prerequisites</span></span>
<span data-ttu-id="13b7f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13b7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13b7f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13b7f-111">Permission type</span></span>|<span data-ttu-id="13b7f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13b7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13b7f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13b7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13b7f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13b7f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13b7f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13b7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13b7f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13b7f-116">Not supported.</span></span>|
|<span data-ttu-id="13b7f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13b7f-117">Application</span></span>|<span data-ttu-id="13b7f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13b7f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13b7f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13b7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="13b7f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13b7f-120">Request headers</span></span>
|<span data-ttu-id="13b7f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13b7f-121">Header</span></span>|<span data-ttu-id="13b7f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="13b7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13b7f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="13b7f-123">Authorization</span></span>|<span data-ttu-id="13b7f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13b7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13b7f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13b7f-125">Accept</span></span>|<span data-ttu-id="13b7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13b7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13b7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13b7f-127">Request body</span></span>
<span data-ttu-id="13b7f-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="13b7f-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="13b7f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="13b7f-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="13b7f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13b7f-130">Property</span></span>|<span data-ttu-id="13b7f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="13b7f-131">Type</span></span>|<span data-ttu-id="13b7f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="13b7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13b7f-133">id</span><span class="sxs-lookup"><span data-stu-id="13b7f-133">id</span></span>|<span data-ttu-id="13b7f-134">String</span><span class="sxs-lookup"><span data-stu-id="13b7f-134">String</span></span>|<span data-ttu-id="13b7f-135">A chave do WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="13b7f-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="13b7f-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="13b7f-136">accessLevel</span></span>|[<span data-ttu-id="13b7f-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="13b7f-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="13b7f-138">Isso indica um nível de acesso para a categoria de dados de privacidade para o qual o aplicativo especificado será fornecido ao.</span><span class="sxs-lookup"><span data-stu-id="13b7f-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="13b7f-139">Os valores possíveis são: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="13b7f-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="13b7f-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="13b7f-140">dataCategory</span></span>|[<span data-ttu-id="13b7f-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="13b7f-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="13b7f-142">Isso indica uma categoria de privacidade de dados ao qual o controle de acesso específico será aplicada.</span><span class="sxs-lookup"><span data-stu-id="13b7f-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="13b7f-143">Os valores possíveis são: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices` .</span><span class="sxs-lookup"><span data-stu-id="13b7f-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="13b7f-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="13b7f-144">appPackageFamilyName</span></span>|<span data-ttu-id="13b7f-145">String</span><span class="sxs-lookup"><span data-stu-id="13b7f-145">String</span></span>|<span data-ttu-id="13b7f-146">O nome da família de pacote de um aplicativo do Windows.</span><span class="sxs-lookup"><span data-stu-id="13b7f-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="13b7f-147">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="13b7f-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="13b7f-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="13b7f-148">appDisplayName</span></span>|<span data-ttu-id="13b7f-149">String</span><span class="sxs-lookup"><span data-stu-id="13b7f-149">String</span></span>|<span data-ttu-id="13b7f-150">O nome da família de pacote de um aplicativo do Windows.</span><span class="sxs-lookup"><span data-stu-id="13b7f-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="13b7f-151">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="13b7f-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="13b7f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="13b7f-152">Response</span></span>
<span data-ttu-id="13b7f-153">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13b7f-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13b7f-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13b7f-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="13b7f-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13b7f-155">Request</span></span>
<span data-ttu-id="13b7f-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13b7f-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="13b7f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="13b7f-157">Response</span></span>
<span data-ttu-id="13b7f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13b7f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





