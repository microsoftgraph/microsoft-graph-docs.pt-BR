---
title: Atualizar deviceManagementDerivedCredentialSettings
description: Atualize as propriedades de um objeto deviceManagementDerivedCredentialSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cec43b49153298789388ec937c8877b4e6fb4ed0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434150"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="b5854-103">Atualizar deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="b5854-103">Update deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="b5854-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5854-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5854-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b5854-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5854-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5854-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5854-107">Atualize as propriedades de [um objeto deviceManagementDerivedCredentialSettings.](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b5854-107">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5854-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b5854-108">Prerequisites</span></span>
<span data-ttu-id="b5854-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5854-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5854-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5854-111">Permission type</span></span>|<span data-ttu-id="b5854-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b5854-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5854-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5854-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b5854-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b5854-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b5854-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5854-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="b5854-116">&nbsp;&nbsp; **Política de Acesso a Recursos**</span><span class="sxs-lookup"><span data-stu-id="b5854-116">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="b5854-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5854-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5854-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5854-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5854-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5854-119">Not supported.</span></span>|
|<span data-ttu-id="b5854-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5854-120">Application</span></span>||
| <span data-ttu-id="b5854-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b5854-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b5854-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5854-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="b5854-123">&nbsp;&nbsp; **Política de Acesso a Recursos**</span><span class="sxs-lookup"><span data-stu-id="b5854-123">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="b5854-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5854-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5854-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5854-125">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b5854-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5854-126">Request headers</span></span>
|<span data-ttu-id="b5854-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5854-127">Header</span></span>|<span data-ttu-id="b5854-128">Valor</span><span class="sxs-lookup"><span data-stu-id="b5854-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5854-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5854-129">Authorization</span></span>|<span data-ttu-id="b5854-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5854-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5854-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b5854-131">Accept</span></span>|<span data-ttu-id="b5854-132">application/json</span><span class="sxs-lookup"><span data-stu-id="b5854-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5854-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5854-133">Request body</span></span>
<span data-ttu-id="b5854-134">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementDerivedCredentialSettings.](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b5854-134">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="b5854-135">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="b5854-135">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="b5854-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5854-136">Property</span></span>|<span data-ttu-id="b5854-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5854-137">Type</span></span>|<span data-ttu-id="b5854-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5854-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5854-139">id</span><span class="sxs-lookup"><span data-stu-id="b5854-139">id</span></span>|<span data-ttu-id="b5854-140">String</span><span class="sxs-lookup"><span data-stu-id="b5854-140">String</span></span>|<span data-ttu-id="b5854-141">Identificador exclusivo da Credencial Derivada</span><span class="sxs-lookup"><span data-stu-id="b5854-141">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="b5854-142">**Política rara**</span><span class="sxs-lookup"><span data-stu-id="b5854-142">**RA Policy**</span></span>|
|<span data-ttu-id="b5854-143">helpUrl</span><span class="sxs-lookup"><span data-stu-id="b5854-143">helpUrl</span></span>|<span data-ttu-id="b5854-144">String</span><span class="sxs-lookup"><span data-stu-id="b5854-144">String</span></span>|<span data-ttu-id="b5854-145">A URL que será acessível aos usuários finais à medida que eles recuperam uma credencial derivada usando o Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="b5854-145">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="b5854-146">displayName</span><span class="sxs-lookup"><span data-stu-id="b5854-146">displayName</span></span>|<span data-ttu-id="b5854-147">String</span><span class="sxs-lookup"><span data-stu-id="b5854-147">String</span></span>|<span data-ttu-id="b5854-148">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="b5854-148">The display name for the profile.</span></span>|
|<span data-ttu-id="b5854-149">emissor</span><span class="sxs-lookup"><span data-stu-id="b5854-149">issuer</span></span>|[<span data-ttu-id="b5854-150">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="b5854-150">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-shared-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="b5854-151">O provedor de credenciais derivado a ser usado.</span><span class="sxs-lookup"><span data-stu-id="b5854-151">The derived credential provider to use.</span></span> <span data-ttu-id="b5854-152">Os valores possíveis são: `intercede`, `entrustDatacard`, `purebred`.</span><span class="sxs-lookup"><span data-stu-id="b5854-152">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="b5854-153">notificationType</span><span class="sxs-lookup"><span data-stu-id="b5854-153">notificationType</span></span>|[<span data-ttu-id="b5854-154">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="b5854-154">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-shared-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="b5854-155">Os métodos usados para informar o usuário final para abrir o Portal da Empresa para fornecer perfis de Wi-Fi, VPN ou email que usam certificados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b5854-155">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="b5854-156">Os valores possíveis são: `none`, `companyPortal`, `email`.</span><span class="sxs-lookup"><span data-stu-id="b5854-156">Possible values are: `none`, `companyPortal`, `email`.</span></span>|


## <a name="response"></a><span data-ttu-id="b5854-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5854-157">Response</span></span>
<span data-ttu-id="b5854-158">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5854-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5854-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5854-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5854-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5854-160">Request</span></span>
<span data-ttu-id="b5854-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5854-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a><span data-ttu-id="b5854-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5854-162">Response</span></span>
<span data-ttu-id="b5854-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5854-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```








