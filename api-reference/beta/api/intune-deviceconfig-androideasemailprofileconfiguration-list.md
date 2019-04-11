---
title: Listar androidEasEmailProfileConfigurations
description: Listar Propriedades e relações dos objetos androidEasEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd8bc6dcc1d5b12ef3104ebbf4895a866c42d0b6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771744"
---
# <a name="list-androideasemailprofileconfigurations"></a><span data-ttu-id="9fec8-103">Listar androidEasEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="9fec8-103">List androidEasEmailProfileConfigurations</span></span>

> <span data-ttu-id="9fec8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9fec8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fec8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9fec8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fec8-106">Listar Propriedades e relações dos objetos [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9fec8-106">List properties and relationships of the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fec8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9fec8-107">Prerequisites</span></span>
<span data-ttu-id="9fec8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fec8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fec8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fec8-110">Permission type</span></span>|<span data-ttu-id="9fec8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9fec8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fec8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fec8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9fec8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fec8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9fec8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fec8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fec8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fec8-115">Not supported.</span></span>|
|<span data-ttu-id="9fec8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fec8-116">Application</span></span>|<span data-ttu-id="9fec8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fec8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fec8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fec8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9fec8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fec8-119">Request headers</span></span>
|<span data-ttu-id="9fec8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9fec8-120">Header</span></span>|<span data-ttu-id="9fec8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9fec8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fec8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fec8-122">Authorization</span></span>|<span data-ttu-id="9fec8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fec8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fec8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9fec8-124">Accept</span></span>|<span data-ttu-id="9fec8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9fec8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fec8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fec8-126">Request body</span></span>
<span data-ttu-id="9fec8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9fec8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fec8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fec8-128">Response</span></span>
<span data-ttu-id="9fec8-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fec8-129">If successful, this method returns a `200 OK` response code and a collection of [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fec8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fec8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fec8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fec8-131">Request</span></span>
<span data-ttu-id="9fec8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fec8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9fec8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fec8-133">Response</span></span>
<span data-ttu-id="9fec8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fec8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1102

{
  "value": [
    {
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
  ]
}
```





