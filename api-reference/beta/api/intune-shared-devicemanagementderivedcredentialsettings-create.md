---
title: Criar deviceManagementDerivedCredentialSettings
description: Criar um novo objeto deviceManagementDerivedCredentialSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a605c0f868eab3deabbc854b27d62cc9e97769b1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194576"
---
# <a name="create-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="344e0-103">Criar deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="344e0-103">Create deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="344e0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="344e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="344e0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="344e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="344e0-106">Criar um novo objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="344e0-106">Create a new [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="344e0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="344e0-107">Prerequisites</span></span>
<span data-ttu-id="344e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="344e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="344e0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="344e0-110">Permission type</span></span>|<span data-ttu-id="344e0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="344e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="344e0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="344e0-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="344e0-113">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="344e0-113">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="344e0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="344e0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="344e0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="344e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="344e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="344e0-116">Not supported.</span></span>|
|<span data-ttu-id="344e0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="344e0-117">Application</span></span>||
|<span data-ttu-id="344e0-118">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="344e0-118">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="344e0-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="344e0-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="344e0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="344e0-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="344e0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="344e0-121">Request headers</span></span>
|<span data-ttu-id="344e0-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="344e0-122">Header</span></span>|<span data-ttu-id="344e0-123">Valor</span><span class="sxs-lookup"><span data-stu-id="344e0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="344e0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="344e0-124">Authorization</span></span>|<span data-ttu-id="344e0-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="344e0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="344e0-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="344e0-126">Accept</span></span>|<span data-ttu-id="344e0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="344e0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="344e0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="344e0-128">Request body</span></span>
<span data-ttu-id="344e0-129">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementDerivedCredentialSettings.</span><span class="sxs-lookup"><span data-stu-id="344e0-129">In the request body, supply a JSON representation for the deviceManagementDerivedCredentialSettings object.</span></span>

<span data-ttu-id="344e0-130">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementDerivedCredentialSettings.</span><span class="sxs-lookup"><span data-stu-id="344e0-130">The following table shows the properties that are required when you create the deviceManagementDerivedCredentialSettings.</span></span>

|<span data-ttu-id="344e0-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="344e0-131">Property</span></span>|<span data-ttu-id="344e0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="344e0-132">Type</span></span>|<span data-ttu-id="344e0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="344e0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="344e0-134">id</span><span class="sxs-lookup"><span data-stu-id="344e0-134">id</span></span>|<span data-ttu-id="344e0-135">String</span><span class="sxs-lookup"><span data-stu-id="344e0-135">String</span></span>|<span data-ttu-id="344e0-136">Identificador exclusivo para a credencial derivada</span><span class="sxs-lookup"><span data-stu-id="344e0-136">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="344e0-137">helpUrl</span><span class="sxs-lookup"><span data-stu-id="344e0-137">helpUrl</span></span>|<span data-ttu-id="344e0-138">String</span><span class="sxs-lookup"><span data-stu-id="344e0-138">String</span></span>|<span data-ttu-id="344e0-139">A URL que será acessível aos usuários finais à medida que eles recuperarem uma credencial derivada usando o portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="344e0-139">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="344e0-140">displayName</span><span class="sxs-lookup"><span data-stu-id="344e0-140">displayName</span></span>|<span data-ttu-id="344e0-141">String</span><span class="sxs-lookup"><span data-stu-id="344e0-141">String</span></span>|<span data-ttu-id="344e0-142">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="344e0-142">The display name for the profile.</span></span>|
|<span data-ttu-id="344e0-143">emissor</span><span class="sxs-lookup"><span data-stu-id="344e0-143">issuer</span></span>|[<span data-ttu-id="344e0-144">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="344e0-144">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-shared-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="344e0-145">O provedor de credenciais derivado a ser usado.</span><span class="sxs-lookup"><span data-stu-id="344e0-145">The derived credential provider to use.</span></span> <span data-ttu-id="344e0-146">Os valores possíveis são: `intercede`, `entrustDatacard`, `purebred`.</span><span class="sxs-lookup"><span data-stu-id="344e0-146">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="344e0-147">notificationType</span><span class="sxs-lookup"><span data-stu-id="344e0-147">notificationType</span></span>|[<span data-ttu-id="344e0-148">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="344e0-148">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-shared-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="344e0-149">Os métodos usados para informar ao usuário final para abrir o portal da empresa para entregar os perfis de Wi-Fi, VPN ou email que usam certificados para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="344e0-149">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="344e0-150">Os valores possíveis são: `none`, `companyPortal`, `email`.</span><span class="sxs-lookup"><span data-stu-id="344e0-150">Possible values are: `none`, `companyPortal`, `email`.</span></span>|



## <a name="response"></a><span data-ttu-id="344e0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="344e0-151">Response</span></span>
<span data-ttu-id="344e0-152">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="344e0-152">If successful, this method returns a `201 Created` response code and a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="344e0-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="344e0-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="344e0-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="344e0-154">Request</span></span>
<span data-ttu-id="344e0-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="344e0-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
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

### <a name="response"></a><span data-ttu-id="344e0-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="344e0-156">Response</span></span>
<span data-ttu-id="344e0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="344e0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





