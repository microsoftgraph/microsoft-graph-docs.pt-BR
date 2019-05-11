---
title: Obter androidForWorkGmailEasConfiguration
description: Leia as propriedades e as relações do objeto androidForWorkGmailEasConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 06b17693afc2421d28a1942a9458989c1f353b96
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933386"
---
# <a name="get-androidforworkgmaileasconfiguration"></a><span data-ttu-id="6c7b7-103">Obter androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c7b7-103">Get androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="6c7b7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c7b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c7b7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c7b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c7b7-106">Leia as propriedades e as relações do objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6c7b7-106">Read properties and relationships of the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c7b7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c7b7-107">Prerequisites</span></span>
<span data-ttu-id="6c7b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c7b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c7b7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c7b7-110">Permission type</span></span>|<span data-ttu-id="6c7b7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c7b7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c7b7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c7b7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c7b7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7b7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6c7b7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c7b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c7b7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c7b7-115">Not supported.</span></span>|
|<span data-ttu-id="6c7b7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c7b7-116">Application</span></span>|<span data-ttu-id="6c7b7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c7b7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c7b7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c7b7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c7b7-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6c7b7-119">Optional query parameters</span></span>
<span data-ttu-id="6c7b7-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6c7b7-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c7b7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7b7-121">Request headers</span></span>
|<span data-ttu-id="6c7b7-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c7b7-122">Header</span></span>|<span data-ttu-id="6c7b7-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6c7b7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c7b7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c7b7-124">Authorization</span></span>|<span data-ttu-id="6c7b7-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c7b7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c7b7-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c7b7-126">Accept</span></span>|<span data-ttu-id="6c7b7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6c7b7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c7b7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7b7-128">Request body</span></span>
<span data-ttu-id="6c7b7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c7b7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c7b7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c7b7-130">Response</span></span>
<span data-ttu-id="6c7b7-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c7b7-131">If successful, this method returns a `200 OK` response code and [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c7b7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c7b7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c7b7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7b7-133">Request</span></span>
<span data-ttu-id="6c7b7-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c7b7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6c7b7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c7b7-135">Response</span></span>
<span data-ttu-id="6c7b7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c7b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 716

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
    "id": "2bafc891-c891-2baf-91c8-af2b91c8af2b",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "authenticationMethod": "certificate",
    "durationOfEmailToSync": "oneDay",
    "emailAddressSource": "primarySmtpAddress",
    "hostName": "Host Name value",
    "requireSsl": true,
    "usernameSource": "userPrincipalName"
  }
}
```




