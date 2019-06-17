---
title: Atualizar deviceManagementDerivedCredentialSettings
description: Atualiza as propriedades de um objeto deviceManagementDerivedCredentialSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0081b43b466439169799d46e0cfcacc341820a3d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967521"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="41cc2-103">Atualizar deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="41cc2-103">Update deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="41cc2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41cc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41cc2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41cc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41cc2-106">Atualiza as propriedades de um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="41cc2-106">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41cc2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41cc2-107">Prerequisites</span></span>
<span data-ttu-id="41cc2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41cc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41cc2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41cc2-110">Permission type</span></span>|<span data-ttu-id="41cc2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41cc2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41cc2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41cc2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41cc2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41cc2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41cc2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41cc2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41cc2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41cc2-115">Not supported.</span></span>|
|<span data-ttu-id="41cc2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41cc2-116">Application</span></span>|<span data-ttu-id="41cc2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41cc2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41cc2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41cc2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="request-headers"></a><span data-ttu-id="41cc2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41cc2-119">Request headers</span></span>
|<span data-ttu-id="41cc2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41cc2-120">Header</span></span>|<span data-ttu-id="41cc2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="41cc2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41cc2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="41cc2-122">Authorization</span></span>|<span data-ttu-id="41cc2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41cc2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41cc2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41cc2-124">Accept</span></span>|<span data-ttu-id="41cc2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41cc2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41cc2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41cc2-126">Request body</span></span>
<span data-ttu-id="41cc2-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="41cc2-127">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="41cc2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="41cc2-128">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="41cc2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41cc2-129">Property</span></span>|<span data-ttu-id="41cc2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="41cc2-130">Type</span></span>|<span data-ttu-id="41cc2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="41cc2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41cc2-132">id</span><span class="sxs-lookup"><span data-stu-id="41cc2-132">id</span></span>|<span data-ttu-id="41cc2-133">String</span><span class="sxs-lookup"><span data-stu-id="41cc2-133">String</span></span>|<span data-ttu-id="41cc2-134">Identificador exclusivo para a credencial derivada</span><span class="sxs-lookup"><span data-stu-id="41cc2-134">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="41cc2-135">helpUrl</span><span class="sxs-lookup"><span data-stu-id="41cc2-135">helpUrl</span></span>|<span data-ttu-id="41cc2-136">String</span><span class="sxs-lookup"><span data-stu-id="41cc2-136">String</span></span>|<span data-ttu-id="41cc2-137">A URL que será acessível aos usuários finais à medida que eles recuperarem uma credencial derivada usando o portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="41cc2-137">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="41cc2-138">displayName</span><span class="sxs-lookup"><span data-stu-id="41cc2-138">displayName</span></span>|<span data-ttu-id="41cc2-139">String</span><span class="sxs-lookup"><span data-stu-id="41cc2-139">String</span></span>|<span data-ttu-id="41cc2-140">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="41cc2-140">The display name for the profile.</span></span>|
|<span data-ttu-id="41cc2-141">emissor</span><span class="sxs-lookup"><span data-stu-id="41cc2-141">issuer</span></span>|[<span data-ttu-id="41cc2-142">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="41cc2-142">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="41cc2-143">O provedor de credenciais derivado a ser usado.</span><span class="sxs-lookup"><span data-stu-id="41cc2-143">The derived credential provider to use.</span></span> <span data-ttu-id="41cc2-144">Os valores possíveis são: `intercede`, `entrustDatacard`, `purebred`.</span><span class="sxs-lookup"><span data-stu-id="41cc2-144">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="41cc2-145">notificationType</span><span class="sxs-lookup"><span data-stu-id="41cc2-145">notificationType</span></span>|[<span data-ttu-id="41cc2-146">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="41cc2-146">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="41cc2-147">Os métodos usados para informar ao usuário final para abrir o portal da empresa para entregar os perfis de Wi-Fi, VPN ou email que usam certificados para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="41cc2-147">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="41cc2-148">Os valores possíveis são: `none`, `companyPortal`, `email`.</span><span class="sxs-lookup"><span data-stu-id="41cc2-148">Possible values are: `none`, `companyPortal`, `email`.</span></span>|



## <a name="response"></a><span data-ttu-id="41cc2-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="41cc2-149">Response</span></span>
<span data-ttu-id="41cc2-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41cc2-150">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41cc2-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41cc2-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="41cc2-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41cc2-152">Request</span></span>
<span data-ttu-id="41cc2-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41cc2-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 241

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
  "issuer": "entrustDatacard",
  "notificationType": "companyPortal"
}
```

### <a name="response"></a><span data-ttu-id="41cc2-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="41cc2-154">Response</span></span>
<span data-ttu-id="41cc2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41cc2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
  "issuer": "entrustDatacard",
  "notificationType": "companyPortal"
}
```





