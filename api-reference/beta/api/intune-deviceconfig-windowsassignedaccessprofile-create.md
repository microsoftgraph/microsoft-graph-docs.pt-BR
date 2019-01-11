---
title: Criar windowsAssignedAccessProfile
description: Crie um novo objeto de windowsAssignedAccessProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4db64578ec2d03f81d10110951a4caf93dc564c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827353"
---
# <a name="create-windowsassignedaccessprofile"></a><span data-ttu-id="299e3-103">Criar windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="299e3-103">Create windowsAssignedAccessProfile</span></span>

> <span data-ttu-id="299e3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="299e3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="299e3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="299e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="299e3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="299e3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="299e3-107">Crie um novo objeto de [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="299e3-107">Create a new [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="299e3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="299e3-108">Prerequisites</span></span>
<span data-ttu-id="299e3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="299e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="299e3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="299e3-111">Permission type</span></span>|<span data-ttu-id="299e3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="299e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="299e3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="299e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="299e3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="299e3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="299e3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="299e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="299e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="299e3-116">Not supported.</span></span>|
|<span data-ttu-id="299e3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="299e3-117">Application</span></span>|<span data-ttu-id="299e3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="299e3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="299e3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="299e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="299e3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="299e3-120">Request headers</span></span>
|<span data-ttu-id="299e3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="299e3-121">Header</span></span>|<span data-ttu-id="299e3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="299e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="299e3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="299e3-123">Authorization</span></span>|<span data-ttu-id="299e3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="299e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="299e3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="299e3-125">Accept</span></span>|<span data-ttu-id="299e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="299e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="299e3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="299e3-127">Request body</span></span>
<span data-ttu-id="299e3-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsAssignedAccessProfile.</span><span class="sxs-lookup"><span data-stu-id="299e3-128">In the request body, supply a JSON representation for the windowsAssignedAccessProfile object.</span></span>

<span data-ttu-id="299e3-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsAssignedAccessProfile.</span><span class="sxs-lookup"><span data-stu-id="299e3-129">The following table shows the properties that are required when you create the windowsAssignedAccessProfile.</span></span>

|<span data-ttu-id="299e3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="299e3-130">Property</span></span>|<span data-ttu-id="299e3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="299e3-131">Type</span></span>|<span data-ttu-id="299e3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="299e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="299e3-133">id</span><span class="sxs-lookup"><span data-stu-id="299e3-133">id</span></span>|<span data-ttu-id="299e3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="299e3-134">String</span></span>|<span data-ttu-id="299e3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="299e3-135">Key of the entity.</span></span>|
|<span data-ttu-id="299e3-136">profileName</span><span class="sxs-lookup"><span data-stu-id="299e3-136">profileName</span></span>|<span data-ttu-id="299e3-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="299e3-137">String</span></span>|<span data-ttu-id="299e3-138">Este é um nome amigável usado para identificar um grupo de aplicativos, o layout desses aplicativos no menu Iniciar e os usuários aos quais essa configuração de quiosque é atribuída.</span><span class="sxs-lookup"><span data-stu-id="299e3-138">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="299e3-139">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="299e3-139">showTaskBar</span></span>|<span data-ttu-id="299e3-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="299e3-140">Boolean</span></span>|<span data-ttu-id="299e3-141">Essa configuração permite que o administrador especificar se a barra de tarefas é mostrada ou não.</span><span class="sxs-lookup"><span data-stu-id="299e3-141">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="299e3-142">appUserModelIds</span><span class="sxs-lookup"><span data-stu-id="299e3-142">appUserModelIds</span></span>|<span data-ttu-id="299e3-143">String collection</span><span class="sxs-lookup"><span data-stu-id="299e3-143">String collection</span></span>|<span data-ttu-id="299e3-144">Estes são os únicos repositório aplicativos do Windows que estarão disponíveis para início no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="299e3-144">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="299e3-145">desktopAppPaths</span><span class="sxs-lookup"><span data-stu-id="299e3-145">desktopAppPaths</span></span>|<span data-ttu-id="299e3-146">String collection</span><span class="sxs-lookup"><span data-stu-id="299e3-146">String collection</span></span>|<span data-ttu-id="299e3-147">Estes são os caminhos dos aplicativos de área de trabalho que estarão disponíveis no menu Iniciar e os aplicativos somente o usuário será capaz de início.</span><span class="sxs-lookup"><span data-stu-id="299e3-147">These are the paths of the Desktop Apps that will be available on the Start menu and the only apps the user will be able to launch.</span></span>|
|<span data-ttu-id="299e3-148">userAccounts</span><span class="sxs-lookup"><span data-stu-id="299e3-148">userAccounts</span></span>|<span data-ttu-id="299e3-149">String collection</span><span class="sxs-lookup"><span data-stu-id="299e3-149">String collection</span></span>|<span data-ttu-id="299e3-150">As contas de usuário que serão bloqueadas para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="299e3-150">The user accounts that will be locked to this kiosk configuration.</span></span>|
|<span data-ttu-id="299e3-151">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="299e3-151">startMenuLayoutXml</span></span>|<span data-ttu-id="299e3-152">Binária</span><span class="sxs-lookup"><span data-stu-id="299e3-152">Binary</span></span>|<span data-ttu-id="299e3-153">Permite que os administradores substituir o layout de início padrão e impede que o usuário alterá-la.</span><span class="sxs-lookup"><span data-stu-id="299e3-153">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="299e3-154">O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout.</span><span class="sxs-lookup"><span data-stu-id="299e3-154"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="299e3-155">XML deve estar em formato binário.</span><span class="sxs-lookup"><span data-stu-id="299e3-155">XML needs to be in Binary format.</span></span>|



## <a name="response"></a><span data-ttu-id="299e3-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="299e3-156">Response</span></span>
<span data-ttu-id="299e3-157">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="299e3-157">If successful, this method returns a `201 Created` response code and a [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="299e3-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="299e3-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="299e3-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="299e3-159">Request</span></span>
<span data-ttu-id="299e3-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="299e3-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles
Content-type: application/json
Content-length: 364

{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
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

### <a name="response"></a><span data-ttu-id="299e3-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="299e3-161">Response</span></span>
<span data-ttu-id="299e3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="299e3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





