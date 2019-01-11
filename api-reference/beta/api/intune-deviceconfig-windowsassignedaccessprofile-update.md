---
title: Atualizar windowsAssignedAccessProfile
description: Atualize as propriedades de um objeto windowsAssignedAccessProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4bfa70208a456d7b7d2a2d0ae524d9edd9508cab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867043"
---
# <a name="update-windowsassignedaccessprofile"></a><span data-ttu-id="196dd-103">Atualizar windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="196dd-103">Update windowsAssignedAccessProfile</span></span>

> <span data-ttu-id="196dd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="196dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="196dd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="196dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="196dd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="196dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="196dd-107">Atualize as propriedades de um objeto [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="196dd-107">Update the properties of a [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="196dd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="196dd-108">Prerequisites</span></span>
<span data-ttu-id="196dd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="196dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="196dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="196dd-111">Permission type</span></span>|<span data-ttu-id="196dd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="196dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="196dd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="196dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="196dd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="196dd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="196dd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="196dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="196dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="196dd-116">Not supported.</span></span>|
|<span data-ttu-id="196dd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="196dd-117">Application</span></span>|<span data-ttu-id="196dd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="196dd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="196dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="196dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="196dd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="196dd-120">Request headers</span></span>
|<span data-ttu-id="196dd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="196dd-121">Header</span></span>|<span data-ttu-id="196dd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="196dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="196dd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="196dd-123">Authorization</span></span>|<span data-ttu-id="196dd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="196dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="196dd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="196dd-125">Accept</span></span>|<span data-ttu-id="196dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="196dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="196dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="196dd-127">Request body</span></span>
<span data-ttu-id="196dd-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="196dd-128">In the request body, supply a JSON representation for the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>

<span data-ttu-id="196dd-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).</span><span class="sxs-lookup"><span data-stu-id="196dd-129">The following table shows the properties that are required when you create the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).</span></span>

|<span data-ttu-id="196dd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="196dd-130">Property</span></span>|<span data-ttu-id="196dd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="196dd-131">Type</span></span>|<span data-ttu-id="196dd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="196dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="196dd-133">id</span><span class="sxs-lookup"><span data-stu-id="196dd-133">id</span></span>|<span data-ttu-id="196dd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="196dd-134">String</span></span>|<span data-ttu-id="196dd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="196dd-135">Key of the entity.</span></span>|
|<span data-ttu-id="196dd-136">profileName</span><span class="sxs-lookup"><span data-stu-id="196dd-136">profileName</span></span>|<span data-ttu-id="196dd-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="196dd-137">String</span></span>|<span data-ttu-id="196dd-138">Este é um nome amigável usado para identificar um grupo de aplicativos, o layout desses aplicativos no menu Iniciar e os usuários aos quais essa configuração de quiosque é atribuída.</span><span class="sxs-lookup"><span data-stu-id="196dd-138">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="196dd-139">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="196dd-139">showTaskBar</span></span>|<span data-ttu-id="196dd-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="196dd-140">Boolean</span></span>|<span data-ttu-id="196dd-141">Essa configuração permite que o administrador especificar se a barra de tarefas é mostrada ou não.</span><span class="sxs-lookup"><span data-stu-id="196dd-141">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="196dd-142">appUserModelIds</span><span class="sxs-lookup"><span data-stu-id="196dd-142">appUserModelIds</span></span>|<span data-ttu-id="196dd-143">String collection</span><span class="sxs-lookup"><span data-stu-id="196dd-143">String collection</span></span>|<span data-ttu-id="196dd-144">Estes são os únicos repositório aplicativos do Windows que estarão disponíveis para início no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="196dd-144">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="196dd-145">desktopAppPaths</span><span class="sxs-lookup"><span data-stu-id="196dd-145">desktopAppPaths</span></span>|<span data-ttu-id="196dd-146">String collection</span><span class="sxs-lookup"><span data-stu-id="196dd-146">String collection</span></span>|<span data-ttu-id="196dd-147">Estes são os caminhos dos aplicativos de área de trabalho que estarão disponíveis no menu Iniciar e os aplicativos somente o usuário será capaz de início.</span><span class="sxs-lookup"><span data-stu-id="196dd-147">These are the paths of the Desktop Apps that will be available on the Start menu and the only apps the user will be able to launch.</span></span>|
|<span data-ttu-id="196dd-148">userAccounts</span><span class="sxs-lookup"><span data-stu-id="196dd-148">userAccounts</span></span>|<span data-ttu-id="196dd-149">String collection</span><span class="sxs-lookup"><span data-stu-id="196dd-149">String collection</span></span>|<span data-ttu-id="196dd-150">As contas de usuário que serão bloqueadas para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="196dd-150">The user accounts that will be locked to this kiosk configuration.</span></span>|
|<span data-ttu-id="196dd-151">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="196dd-151">startMenuLayoutXml</span></span>|<span data-ttu-id="196dd-152">Binária</span><span class="sxs-lookup"><span data-stu-id="196dd-152">Binary</span></span>|<span data-ttu-id="196dd-153">Permite que os administradores substituir o layout de início padrão e impede que o usuário alterá-la.</span><span class="sxs-lookup"><span data-stu-id="196dd-153">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="196dd-154">O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout.</span><span class="sxs-lookup"><span data-stu-id="196dd-154"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="196dd-155">XML deve estar em formato binário.</span><span class="sxs-lookup"><span data-stu-id="196dd-155">XML needs to be in Binary format.</span></span>|



## <a name="response"></a><span data-ttu-id="196dd-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="196dd-156">Response</span></span>
<span data-ttu-id="196dd-157">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="196dd-157">If successful, this method returns a `200 OK` response code and an updated [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="196dd-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="196dd-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="196dd-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="196dd-159">Request</span></span>
<span data-ttu-id="196dd-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="196dd-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
Content-type: application/json
Content-length: 297

{
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```

### <a name="response"></a><span data-ttu-id="196dd-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="196dd-161">Response</span></span>
<span data-ttu-id="196dd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="196dd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 413

{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```





