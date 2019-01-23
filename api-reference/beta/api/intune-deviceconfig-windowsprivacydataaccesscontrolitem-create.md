---
title: Criar windowsPrivacyDataAccessControlItem
description: Crie um novo objeto de windowsPrivacyDataAccessControlItem.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e7b78a113134b4d268df3c759dfd7dc700759a35
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405580"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="43189-103">Criar windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="43189-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="43189-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="43189-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="43189-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="43189-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43189-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="43189-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43189-107">Crie um novo objeto de [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="43189-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43189-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43189-108">Prerequisites</span></span>
<span data-ttu-id="43189-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="43189-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="43189-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43189-111">Permission type</span></span>|<span data-ttu-id="43189-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43189-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43189-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43189-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43189-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43189-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43189-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43189-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43189-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43189-116">Not supported.</span></span>|
|<span data-ttu-id="43189-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43189-117">Application</span></span>|<span data-ttu-id="43189-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43189-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43189-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43189-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="43189-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43189-120">Request headers</span></span>
|<span data-ttu-id="43189-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43189-121">Header</span></span>|<span data-ttu-id="43189-122">Valor</span><span class="sxs-lookup"><span data-stu-id="43189-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43189-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="43189-123">Authorization</span></span>|<span data-ttu-id="43189-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43189-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43189-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43189-125">Accept</span></span>|<span data-ttu-id="43189-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43189-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43189-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43189-127">Request body</span></span>
<span data-ttu-id="43189-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="43189-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="43189-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="43189-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="43189-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43189-130">Property</span></span>|<span data-ttu-id="43189-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="43189-131">Type</span></span>|<span data-ttu-id="43189-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="43189-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43189-133">id</span><span class="sxs-lookup"><span data-stu-id="43189-133">id</span></span>|<span data-ttu-id="43189-134">String</span><span class="sxs-lookup"><span data-stu-id="43189-134">String</span></span>|<span data-ttu-id="43189-135">A chave do WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="43189-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="43189-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="43189-136">accessLevel</span></span>|[<span data-ttu-id="43189-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="43189-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="43189-138">Isso indica um nível de acesso para a categoria de dados de privacidade para o qual o aplicativo especificado será fornecido ao.</span><span class="sxs-lookup"><span data-stu-id="43189-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="43189-139">Os valores possíveis são: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="43189-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="43189-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="43189-140">dataCategory</span></span>|[<span data-ttu-id="43189-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="43189-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="43189-142">Isso indica uma categoria de privacidade de dados ao qual o controle de acesso específico será aplicada.</span><span class="sxs-lookup"><span data-stu-id="43189-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="43189-143">Os valores possíveis são: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices` .</span><span class="sxs-lookup"><span data-stu-id="43189-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="43189-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="43189-144">appPackageFamilyName</span></span>|<span data-ttu-id="43189-145">String</span><span class="sxs-lookup"><span data-stu-id="43189-145">String</span></span>|<span data-ttu-id="43189-146">O nome da família de pacote de um aplicativo do Windows.</span><span class="sxs-lookup"><span data-stu-id="43189-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="43189-147">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="43189-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="43189-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="43189-148">appDisplayName</span></span>|<span data-ttu-id="43189-149">String</span><span class="sxs-lookup"><span data-stu-id="43189-149">String</span></span>|<span data-ttu-id="43189-150">O nome da família de pacote de um aplicativo do Windows.</span><span class="sxs-lookup"><span data-stu-id="43189-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="43189-151">Quando definido, o nível de acesso se aplica ao aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="43189-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="43189-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="43189-152">Response</span></span>
<span data-ttu-id="43189-153">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43189-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43189-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43189-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="43189-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43189-155">Request</span></span>
<span data-ttu-id="43189-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43189-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43189-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="43189-157">Response</span></span>
<span data-ttu-id="43189-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43189-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




