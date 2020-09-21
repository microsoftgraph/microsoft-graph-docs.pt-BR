---
title: Listar iosLobAppProvisioningConfigurations
description: Listar Propriedades e relações dos objetos iosLobAppProvisioningConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 819ab16f043c7e556b664cf38f2843d3788cbe43
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036160"
---
# <a name="list-ioslobappprovisioningconfigurations"></a><span data-ttu-id="65f13-103">Listar iosLobAppProvisioningConfigurations</span><span class="sxs-lookup"><span data-stu-id="65f13-103">List iosLobAppProvisioningConfigurations</span></span>

<span data-ttu-id="65f13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65f13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65f13-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65f13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65f13-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65f13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65f13-107">Listar Propriedades e relações dos objetos [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="65f13-107">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65f13-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="65f13-108">Prerequisites</span></span>
<span data-ttu-id="65f13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65f13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65f13-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65f13-111">Permission type</span></span>|<span data-ttu-id="65f13-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="65f13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65f13-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65f13-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="65f13-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="65f13-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="65f13-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="65f13-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="65f13-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="65f13-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="65f13-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="65f13-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="65f13-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65f13-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65f13-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65f13-119">Not supported.</span></span>|
|<span data-ttu-id="65f13-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65f13-120">Application</span></span>||
| <span data-ttu-id="65f13-121">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="65f13-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="65f13-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="65f13-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="65f13-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="65f13-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="65f13-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="65f13-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65f13-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65f13-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="65f13-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65f13-126">Request headers</span></span>
|<span data-ttu-id="65f13-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65f13-127">Header</span></span>|<span data-ttu-id="65f13-128">Valor</span><span class="sxs-lookup"><span data-stu-id="65f13-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65f13-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="65f13-129">Authorization</span></span>|<span data-ttu-id="65f13-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65f13-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65f13-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="65f13-131">Accept</span></span>|<span data-ttu-id="65f13-132">application/json</span><span class="sxs-lookup"><span data-stu-id="65f13-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65f13-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65f13-133">Request body</span></span>
<span data-ttu-id="65f13-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="65f13-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65f13-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="65f13-135">Response</span></span>
<span data-ttu-id="65f13-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65f13-136">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65f13-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65f13-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="65f13-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65f13-138">Request</span></span>
<span data-ttu-id="65f13-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65f13-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
```

### <a name="response"></a><span data-ttu-id="65f13-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="65f13-140">Response</span></span>
<span data-ttu-id="65f13-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65f13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 632

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
      "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA==",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```









