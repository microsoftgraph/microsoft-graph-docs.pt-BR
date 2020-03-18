---
title: Atualizar deviceManagementDerivedCredentialSettings
description: Atualiza as propriedades de um objeto deviceManagementDerivedCredentialSettings.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 534b388975f40e269f006414a6dd39885211f7aa
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800995"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="d7c69-103">Atualizar deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="d7c69-103">Update deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="d7c69-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7c69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7c69-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7c69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7c69-106">Atualiza as propriedades de um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="d7c69-106">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7c69-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7c69-107">Prerequisites</span></span>
<span data-ttu-id="d7c69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7c69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7c69-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7c69-110">Permission type</span></span>|<span data-ttu-id="d7c69-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7c69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7c69-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7c69-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d7c69-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d7c69-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d7c69-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c69-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="d7c69-115">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="d7c69-115">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="d7c69-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c69-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7c69-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7c69-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7c69-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7c69-118">Not supported.</span></span>|
|<span data-ttu-id="d7c69-119">Application</span><span class="sxs-lookup"><span data-stu-id="d7c69-119">Application</span></span>||
| <span data-ttu-id="d7c69-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d7c69-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d7c69-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c69-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="d7c69-122">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="d7c69-122">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="d7c69-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c69-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7c69-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7c69-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="request-headers"></a><span data-ttu-id="d7c69-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c69-125">Request headers</span></span>
|<span data-ttu-id="d7c69-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7c69-126">Header</span></span>|<span data-ttu-id="d7c69-127">Valor</span><span class="sxs-lookup"><span data-stu-id="d7c69-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7c69-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7c69-128">Authorization</span></span>|<span data-ttu-id="d7c69-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7c69-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7c69-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7c69-130">Accept</span></span>|<span data-ttu-id="d7c69-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d7c69-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7c69-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c69-132">Request body</span></span>
<span data-ttu-id="d7c69-133">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="d7c69-133">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="d7c69-134">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="d7c69-134">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="d7c69-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7c69-135">Property</span></span>|<span data-ttu-id="d7c69-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7c69-136">Type</span></span>|<span data-ttu-id="d7c69-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7c69-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7c69-138">id</span><span class="sxs-lookup"><span data-stu-id="d7c69-138">id</span></span>|<span data-ttu-id="d7c69-139">String</span><span class="sxs-lookup"><span data-stu-id="d7c69-139">String</span></span>|<span data-ttu-id="d7c69-140">Identificador exclusivo para a credencial derivada</span><span class="sxs-lookup"><span data-stu-id="d7c69-140">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="d7c69-141">**Política de RA**</span><span class="sxs-lookup"><span data-stu-id="d7c69-141">**RA Policy**</span></span>|
|<span data-ttu-id="d7c69-142">helpUrl</span><span class="sxs-lookup"><span data-stu-id="d7c69-142">helpUrl</span></span>|<span data-ttu-id="d7c69-143">String</span><span class="sxs-lookup"><span data-stu-id="d7c69-143">String</span></span>|<span data-ttu-id="d7c69-144">A URL que será acessível aos usuários finais à medida que eles recuperarem uma credencial derivada usando o portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="d7c69-144">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="d7c69-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d7c69-145">displayName</span></span>|<span data-ttu-id="d7c69-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7c69-146">String</span></span>|<span data-ttu-id="d7c69-147">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="d7c69-147">The display name for the profile.</span></span>|
|<span data-ttu-id="d7c69-148">emissor</span><span class="sxs-lookup"><span data-stu-id="d7c69-148">issuer</span></span>|<span data-ttu-id="d7c69-149">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="d7c69-149">deviceManagementDerivedCredentialIssuer</span></span>|<span data-ttu-id="d7c69-150">O provedor de credenciais derivado a ser usado.</span><span class="sxs-lookup"><span data-stu-id="d7c69-150">The derived credential provider to use.</span></span> <span data-ttu-id="d7c69-151">Os valores possíveis são: `intercede`, `entrustDatacard`, `purebred`.</span><span class="sxs-lookup"><span data-stu-id="d7c69-151">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="d7c69-152">notificationType</span><span class="sxs-lookup"><span data-stu-id="d7c69-152">notificationType</span></span>|<span data-ttu-id="d7c69-153">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="d7c69-153">deviceManagementDerivedCredentialNotificationType</span></span>|<span data-ttu-id="d7c69-154">Os métodos usados para informar ao usuário final para abrir o portal da empresa para entregar os perfis de Wi-Fi, VPN ou email que usam certificados para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d7c69-154">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="d7c69-155">Os valores possíveis são: `none`, `companyPortal`, `email`.</span><span class="sxs-lookup"><span data-stu-id="d7c69-155">Possible values are: `none`, `companyPortal`, `email`.</span></span>|


## <a name="response"></a><span data-ttu-id="d7c69-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7c69-156">Response</span></span>
<span data-ttu-id="d7c69-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7c69-157">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7c69-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7c69-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7c69-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c69-159">Request</span></span>
<span data-ttu-id="d7c69-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7c69-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a><span data-ttu-id="d7c69-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7c69-161">Response</span></span>
<span data-ttu-id="d7c69-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7c69-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```








