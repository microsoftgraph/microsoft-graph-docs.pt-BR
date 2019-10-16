---
title: Listar iosLobAppProvisioningConfigurations
description: Listar Propriedades e relações dos objetos iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6cb6f5ccde71db36ac02bedb7847ed43b3d060dd
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538109"
---
# <a name="list-ioslobappprovisioningconfigurations"></a><span data-ttu-id="53445-103">Listar iosLobAppProvisioningConfigurations</span><span class="sxs-lookup"><span data-stu-id="53445-103">List iosLobAppProvisioningConfigurations</span></span>

> <span data-ttu-id="53445-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53445-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53445-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53445-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53445-106">Listar Propriedades e relações dos objetos [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="53445-106">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53445-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53445-107">Prerequisites</span></span>
<span data-ttu-id="53445-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53445-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53445-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53445-110">Permission type</span></span>|<span data-ttu-id="53445-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53445-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53445-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53445-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="53445-113">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="53445-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="53445-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="53445-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="53445-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="53445-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="53445-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="53445-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="53445-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53445-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53445-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53445-118">Not supported.</span></span>|
|<span data-ttu-id="53445-119">Application</span><span class="sxs-lookup"><span data-stu-id="53445-119">Application</span></span>||
| <span data-ttu-id="53445-120">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="53445-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="53445-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="53445-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="53445-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="53445-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="53445-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="53445-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53445-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53445-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="53445-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53445-125">Request headers</span></span>
|<span data-ttu-id="53445-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53445-126">Header</span></span>|<span data-ttu-id="53445-127">Valor</span><span class="sxs-lookup"><span data-stu-id="53445-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53445-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="53445-128">Authorization</span></span>|<span data-ttu-id="53445-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53445-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53445-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53445-130">Accept</span></span>|<span data-ttu-id="53445-131">application/json</span><span class="sxs-lookup"><span data-stu-id="53445-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53445-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53445-132">Request body</span></span>
<span data-ttu-id="53445-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="53445-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53445-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="53445-134">Response</span></span>
<span data-ttu-id="53445-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53445-135">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53445-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53445-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="53445-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53445-137">Request</span></span>
<span data-ttu-id="53445-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53445-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
```

### <a name="response"></a><span data-ttu-id="53445-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="53445-139">Response</span></span>
<span data-ttu-id="53445-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53445-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






