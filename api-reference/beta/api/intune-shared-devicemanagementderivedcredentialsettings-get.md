---
title: Obter deviceManagementDerivedCredentialSettings
description: Leia as propriedades e as relações do objeto deviceManagementDerivedCredentialSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5519ae01e8091b7f7b55b15b90495d8167ab0c36
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939932"
---
# <a name="get-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="04b8f-103">Obter deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="04b8f-103">Get deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="04b8f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04b8f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04b8f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04b8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04b8f-106">Leia as propriedades e as relações do objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="04b8f-106">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04b8f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04b8f-107">Prerequisites</span></span>
<span data-ttu-id="04b8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04b8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04b8f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04b8f-110">Permission type</span></span>|<span data-ttu-id="04b8f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04b8f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04b8f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04b8f-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="04b8f-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="04b8f-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="04b8f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b8f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="04b8f-115">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="04b8f-115">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="04b8f-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b8f-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="04b8f-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04b8f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04b8f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04b8f-118">Not supported.</span></span>|
|<span data-ttu-id="04b8f-119">Application</span><span class="sxs-lookup"><span data-stu-id="04b8f-119">Application</span></span>||
|<span data-ttu-id="04b8f-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="04b8f-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="04b8f-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b8f-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="04b8f-122">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="04b8f-122">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="04b8f-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b8f-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04b8f-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04b8f-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04b8f-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="04b8f-125">Optional query parameters</span></span>
<span data-ttu-id="04b8f-126">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="04b8f-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04b8f-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04b8f-127">Request headers</span></span>
|<span data-ttu-id="04b8f-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04b8f-128">Header</span></span>|<span data-ttu-id="04b8f-129">Valor</span><span class="sxs-lookup"><span data-stu-id="04b8f-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04b8f-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="04b8f-130">Authorization</span></span>|<span data-ttu-id="04b8f-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04b8f-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04b8f-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04b8f-132">Accept</span></span>|<span data-ttu-id="04b8f-133">application/json</span><span class="sxs-lookup"><span data-stu-id="04b8f-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04b8f-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04b8f-134">Request body</span></span>
<span data-ttu-id="04b8f-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04b8f-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04b8f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="04b8f-136">Response</span></span>
<span data-ttu-id="04b8f-137">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04b8f-137">If successful, this method returns a `200 OK` response code and [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04b8f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04b8f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="04b8f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04b8f-139">Request</span></span>
<span data-ttu-id="04b8f-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04b8f-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
```

### <a name="response"></a><span data-ttu-id="04b8f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="04b8f-141">Response</span></span>
<span data-ttu-id="04b8f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04b8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 155

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
    "id": "bc650741-0741-bc65-4107-65bc410765bc"
  }
}






