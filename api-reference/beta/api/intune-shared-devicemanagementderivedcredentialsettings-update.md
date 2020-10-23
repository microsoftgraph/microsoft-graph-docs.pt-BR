---
title: Atualizar deviceManagementDerivedCredentialSettings
description: Atualiza as propriedades de um objeto deviceManagementDerivedCredentialSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b611c63d069e0abbf74490406c52af76bf5efa1a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706286"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="d9ab9-103">Atualizar deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="d9ab9-103">Update deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="d9ab9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9ab9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9ab9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9ab9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9ab9-107">Atualiza as propriedades de um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="d9ab9-107">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9ab9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9ab9-108">Prerequisites</span></span>
<span data-ttu-id="d9ab9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9ab9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9ab9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9ab9-111">Permission type</span></span>|<span data-ttu-id="d9ab9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9ab9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9ab9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9ab9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d9ab9-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d9ab9-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d9ab9-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9ab9-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="d9ab9-116">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="d9ab9-116">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="d9ab9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9ab9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9ab9-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9ab9-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9ab9-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-119">Not supported.</span></span>|
|<span data-ttu-id="d9ab9-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9ab9-120">Application</span></span>||
| <span data-ttu-id="d9ab9-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d9ab9-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d9ab9-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9ab9-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="d9ab9-123">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="d9ab9-123">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="d9ab9-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9ab9-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9ab9-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9ab9-125">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d9ab9-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9ab9-126">Request headers</span></span>
|<span data-ttu-id="d9ab9-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9ab9-127">Header</span></span>|<span data-ttu-id="d9ab9-128">Valor</span><span class="sxs-lookup"><span data-stu-id="d9ab9-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9ab9-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9ab9-129">Authorization</span></span>|<span data-ttu-id="d9ab9-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9ab9-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9ab9-131">Accept</span></span>|<span data-ttu-id="d9ab9-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d9ab9-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9ab9-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9ab9-133">Request body</span></span>
<span data-ttu-id="d9ab9-134">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="d9ab9-134">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="d9ab9-135">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="d9ab9-135">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="d9ab9-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9ab9-136">Property</span></span>|<span data-ttu-id="d9ab9-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9ab9-137">Type</span></span>|<span data-ttu-id="d9ab9-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9ab9-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9ab9-139">id</span><span class="sxs-lookup"><span data-stu-id="d9ab9-139">id</span></span>|<span data-ttu-id="d9ab9-140">String</span><span class="sxs-lookup"><span data-stu-id="d9ab9-140">String</span></span>|<span data-ttu-id="d9ab9-141">Identificador exclusivo para a credencial derivada</span><span class="sxs-lookup"><span data-stu-id="d9ab9-141">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="d9ab9-142">**Política de RA**</span><span class="sxs-lookup"><span data-stu-id="d9ab9-142">**RA Policy**</span></span>|
|<span data-ttu-id="d9ab9-143">helpUrl</span><span class="sxs-lookup"><span data-stu-id="d9ab9-143">helpUrl</span></span>|<span data-ttu-id="d9ab9-144">String</span><span class="sxs-lookup"><span data-stu-id="d9ab9-144">String</span></span>|<span data-ttu-id="d9ab9-145">A URL que será acessível aos usuários finais à medida que eles recuperarem uma credencial derivada usando o portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-145">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="d9ab9-146">displayName</span><span class="sxs-lookup"><span data-stu-id="d9ab9-146">displayName</span></span>|<span data-ttu-id="d9ab9-147">String</span><span class="sxs-lookup"><span data-stu-id="d9ab9-147">String</span></span>|<span data-ttu-id="d9ab9-148">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-148">The display name for the profile.</span></span>|
|<span data-ttu-id="d9ab9-149">emissor</span><span class="sxs-lookup"><span data-stu-id="d9ab9-149">issuer</span></span>|<span data-ttu-id="d9ab9-150">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="d9ab9-150">deviceManagementDerivedCredentialIssuer</span></span>|<span data-ttu-id="d9ab9-151">O provedor de credenciais derivado a ser usado.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-151">The derived credential provider to use.</span></span> <span data-ttu-id="d9ab9-152">Os valores possíveis são: `intercede`, `entrustDatacard`, `purebred`.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-152">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="d9ab9-153">notificationType</span><span class="sxs-lookup"><span data-stu-id="d9ab9-153">notificationType</span></span>|<span data-ttu-id="d9ab9-154">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="d9ab9-154">deviceManagementDerivedCredentialNotificationType</span></span>|<span data-ttu-id="d9ab9-155">Os métodos usados para informar ao usuário final para abrir o portal da empresa para entregar os perfis de Wi-Fi, VPN ou email que usam certificados para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-155">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="d9ab9-156">Os valores possíveis são: `none`, `companyPortal`, `email`.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-156">Possible values are: `none`, `companyPortal`, `email`.</span></span>|


## <a name="response"></a><span data-ttu-id="d9ab9-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9ab9-157">Response</span></span>
<span data-ttu-id="d9ab9-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9ab9-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9ab9-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9ab9-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9ab9-160">Request</span></span>
<span data-ttu-id="d9ab9-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a><span data-ttu-id="d9ab9-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9ab9-162">Response</span></span>
<span data-ttu-id="d9ab9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9ab9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```









