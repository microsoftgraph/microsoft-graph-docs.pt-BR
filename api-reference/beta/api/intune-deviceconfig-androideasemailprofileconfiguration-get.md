---
title: Obter androidEasEmailProfileConfiguration
description: Leia as propriedades e as relações do objeto androidEasEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9239ade28da569fa3a6954745833669b7d4a78bf
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976355"
---
# <a name="get-androideasemailprofileconfiguration"></a><span data-ttu-id="cf50a-103">Obter androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf50a-103">Get androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="cf50a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf50a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf50a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf50a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf50a-106">Leia as propriedades e as relações do objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cf50a-106">Read properties and relationships of the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf50a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf50a-107">Prerequisites</span></span>
<span data-ttu-id="cf50a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf50a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf50a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf50a-110">Permission type</span></span>|<span data-ttu-id="cf50a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf50a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf50a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf50a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf50a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf50a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cf50a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf50a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf50a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf50a-115">Not supported.</span></span>|
|<span data-ttu-id="cf50a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf50a-116">Application</span></span>|<span data-ttu-id="cf50a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf50a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf50a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf50a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf50a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cf50a-119">Optional query parameters</span></span>
<span data-ttu-id="cf50a-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cf50a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf50a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf50a-121">Request headers</span></span>
|<span data-ttu-id="cf50a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf50a-122">Header</span></span>|<span data-ttu-id="cf50a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cf50a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf50a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf50a-124">Authorization</span></span>|<span data-ttu-id="cf50a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf50a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf50a-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf50a-126">Accept</span></span>|<span data-ttu-id="cf50a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cf50a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf50a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf50a-128">Request body</span></span>
<span data-ttu-id="cf50a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf50a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf50a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf50a-130">Response</span></span>
<span data-ttu-id="cf50a-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf50a-131">If successful, this method returns a `200 OK` response code and [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf50a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf50a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf50a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf50a-133">Request</span></span>
<span data-ttu-id="cf50a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf50a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="cf50a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf50a-135">Response</span></span>
<span data-ttu-id="cf50a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf50a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1036

{
  "value": {
    "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
    "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountName": "Account Name value",
    "authenticationMethod": "certificate",
    "syncCalendar": true,
    "syncContacts": true,
    "syncTasks": true,
    "syncNotes": true,
    "durationOfEmailToSync": "oneDay",
    "emailAddressSource": "primarySmtpAddress",
    "emailSyncSchedule": "asMessagesArrive",
    "hostName": "Host Name value",
    "requireSmime": true,
    "requireSsl": true,
    "usernameSource": "userPrincipalName",
    "userDomainNameSource": "netBiosDomainName",
    "customDomainName": "Custom Domain Name value"
  }
}
```




