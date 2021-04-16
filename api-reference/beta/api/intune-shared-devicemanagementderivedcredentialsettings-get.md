---
title: Obter deviceManagementDerivedCredentialSettings
description: Leia propriedades e relações do objeto deviceManagementDerivedCredentialSettings.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf8671aa57a9aa85627dc895370008af93998e1f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867487"
---
# <a name="get-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="2685e-103">Obter deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="2685e-103">Get deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="2685e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2685e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2685e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2685e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2685e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2685e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2685e-107">Leia propriedades e relações do [objeto deviceManagementDerivedCredentialSettings.](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2685e-107">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2685e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2685e-108">Prerequisites</span></span>
<span data-ttu-id="2685e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2685e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2685e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2685e-111">Permission type</span></span>|<span data-ttu-id="2685e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2685e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2685e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2685e-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="2685e-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="2685e-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2685e-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2685e-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2685e-116">&nbsp;&nbsp; **Política de Acesso a Recursos**</span><span class="sxs-lookup"><span data-stu-id="2685e-116">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="2685e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2685e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2685e-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2685e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2685e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2685e-119">Not supported.</span></span>|
|<span data-ttu-id="2685e-120">Application</span><span class="sxs-lookup"><span data-stu-id="2685e-120">Application</span></span>||
|<span data-ttu-id="2685e-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="2685e-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2685e-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2685e-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2685e-123">&nbsp;&nbsp; **Política de Acesso a Recursos**</span><span class="sxs-lookup"><span data-stu-id="2685e-123">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="2685e-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2685e-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2685e-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2685e-125">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="2685e-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2685e-126">Optional query parameters</span></span>
<span data-ttu-id="2685e-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2685e-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2685e-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2685e-128">Request headers</span></span>
|<span data-ttu-id="2685e-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2685e-129">Header</span></span>|<span data-ttu-id="2685e-130">Valor</span><span class="sxs-lookup"><span data-stu-id="2685e-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2685e-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="2685e-131">Authorization</span></span>|<span data-ttu-id="2685e-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2685e-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2685e-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2685e-133">Accept</span></span>|<span data-ttu-id="2685e-134">application/json</span><span class="sxs-lookup"><span data-stu-id="2685e-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2685e-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2685e-135">Request body</span></span>
<span data-ttu-id="2685e-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2685e-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2685e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2685e-137">Response</span></span>
<span data-ttu-id="2685e-138">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2685e-138">If successful, this method returns a `200 OK` response code and [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2685e-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2685e-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="2685e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2685e-140">Request</span></span>
<span data-ttu-id="2685e-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2685e-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
```

### <a name="response"></a><span data-ttu-id="2685e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2685e-142">Response</span></span>
<span data-ttu-id="2685e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2685e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
```




