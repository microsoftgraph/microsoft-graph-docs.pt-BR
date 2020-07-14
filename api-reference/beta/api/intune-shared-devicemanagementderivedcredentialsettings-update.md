---
title: Atualizar deviceManagementDerivedCredentialSettings
description: Atualiza as propriedades de um objeto deviceManagementDerivedCredentialSettings.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cf0460b25c3be317d9aebe7a91a02f7d2ae9f534
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123558"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="1ee5f-103">Atualizar deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="1ee5f-103">Update deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="1ee5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ee5f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ee5f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ee5f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ee5f-107">Atualiza as propriedades de um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="1ee5f-107">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ee5f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ee5f-108">Prerequisites</span></span>
<span data-ttu-id="1ee5f-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1ee5f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ee5f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ee5f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ee5f-111">Permission type</span></span>|<span data-ttu-id="1ee5f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ee5f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ee5f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ee5f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1ee5f-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="1ee5f-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="1ee5f-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee5f-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="1ee5f-116">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="1ee5f-116">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="1ee5f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee5f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ee5f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ee5f-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ee5f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-119">Not supported.</span></span>|
|<span data-ttu-id="1ee5f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ee5f-120">Application</span></span>||
| <span data-ttu-id="1ee5f-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="1ee5f-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="1ee5f-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee5f-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="1ee5f-123">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="1ee5f-123">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="1ee5f-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee5f-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ee5f-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ee5f-125">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1ee5f-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ee5f-126">Request headers</span></span>
|<span data-ttu-id="1ee5f-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ee5f-127">Header</span></span>|<span data-ttu-id="1ee5f-128">Valor</span><span class="sxs-lookup"><span data-stu-id="1ee5f-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ee5f-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ee5f-129">Authorization</span></span>|<span data-ttu-id="1ee5f-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ee5f-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ee5f-131">Accept</span></span>|<span data-ttu-id="1ee5f-132">application/json</span><span class="sxs-lookup"><span data-stu-id="1ee5f-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ee5f-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ee5f-133">Request body</span></span>
<span data-ttu-id="1ee5f-134">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="1ee5f-134">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="1ee5f-135">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="1ee5f-135">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="1ee5f-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ee5f-136">Property</span></span>|<span data-ttu-id="1ee5f-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ee5f-137">Type</span></span>|<span data-ttu-id="1ee5f-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ee5f-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ee5f-139">id</span><span class="sxs-lookup"><span data-stu-id="1ee5f-139">id</span></span>|<span data-ttu-id="1ee5f-140">String</span><span class="sxs-lookup"><span data-stu-id="1ee5f-140">String</span></span>|<span data-ttu-id="1ee5f-141">Identificador exclusivo para a credencial derivada</span><span class="sxs-lookup"><span data-stu-id="1ee5f-141">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="1ee5f-142">**Política de RA**</span><span class="sxs-lookup"><span data-stu-id="1ee5f-142">**RA Policy**</span></span>|
|<span data-ttu-id="1ee5f-143">helpUrl</span><span class="sxs-lookup"><span data-stu-id="1ee5f-143">helpUrl</span></span>|<span data-ttu-id="1ee5f-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ee5f-144">String</span></span>|<span data-ttu-id="1ee5f-145">A URL que será acessível aos usuários finais à medida que eles recuperarem uma credencial derivada usando o portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-145">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="1ee5f-146">displayName</span><span class="sxs-lookup"><span data-stu-id="1ee5f-146">displayName</span></span>|<span data-ttu-id="1ee5f-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ee5f-147">String</span></span>|<span data-ttu-id="1ee5f-148">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-148">The display name for the profile.</span></span>|
|<span data-ttu-id="1ee5f-149">emissor</span><span class="sxs-lookup"><span data-stu-id="1ee5f-149">issuer</span></span>|[<span data-ttu-id="1ee5f-150">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="1ee5f-150">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-shared-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="1ee5f-151">O provedor de credenciais derivado a ser usado.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-151">The derived credential provider to use.</span></span> <span data-ttu-id="1ee5f-152">Os valores possíveis são: `intercede`, `entrustDatacard`, `purebred`.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-152">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="1ee5f-153">notificationType</span><span class="sxs-lookup"><span data-stu-id="1ee5f-153">notificationType</span></span>|[<span data-ttu-id="1ee5f-154">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="1ee5f-154">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-shared-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="1ee5f-155">Os métodos usados para informar ao usuário final para abrir o portal da empresa para entregar os perfis de Wi-Fi, VPN ou email que usam certificados para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-155">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="1ee5f-156">Os valores possíveis são: `none`, `companyPortal`, `email`.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-156">Possible values are: `none`, `companyPortal`, `email`.</span></span>|


## <a name="response"></a><span data-ttu-id="1ee5f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ee5f-157">Response</span></span>
<span data-ttu-id="1ee5f-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ee5f-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ee5f-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ee5f-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ee5f-160">Request</span></span>
<span data-ttu-id="1ee5f-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a><span data-ttu-id="1ee5f-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ee5f-162">Response</span></span>
<span data-ttu-id="1ee5f-163">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-163">Here is an example of the response.</span></span> <span data-ttu-id="1ee5f-164">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1ee5f-165">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1ee5f-165">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```







