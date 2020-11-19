---
title: Listar iosLobAppProvisioningConfigurations
description: Listar Propriedades e relações dos objetos iosLobAppProvisioningConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02f81a8c19f5656fed51074b0f0564c58c953666
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49261983"
---
# <a name="list-ioslobappprovisioningconfigurations"></a><span data-ttu-id="c7dc8-103">Listar iosLobAppProvisioningConfigurations</span><span class="sxs-lookup"><span data-stu-id="c7dc8-103">List iosLobAppProvisioningConfigurations</span></span>

<span data-ttu-id="c7dc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7dc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7dc8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7dc8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7dc8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7dc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7dc8-107">Listar Propriedades e relações dos objetos [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c7dc8-107">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7dc8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7dc8-108">Prerequisites</span></span>
<span data-ttu-id="c7dc8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7dc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7dc8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7dc8-111">Permission type</span></span>|<span data-ttu-id="c7dc8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7dc8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7dc8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7dc8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c7dc8-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="c7dc8-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="c7dc8-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7dc8-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="c7dc8-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="c7dc8-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c7dc8-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7dc8-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c7dc8-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7dc8-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7dc8-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7dc8-119">Not supported.</span></span>|
|<span data-ttu-id="c7dc8-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7dc8-120">Application</span></span>||
| <span data-ttu-id="c7dc8-121">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="c7dc8-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="c7dc8-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7dc8-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="c7dc8-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="c7dc8-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c7dc8-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7dc8-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7dc8-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7dc8-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c7dc8-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7dc8-126">Request headers</span></span>
|<span data-ttu-id="c7dc8-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7dc8-127">Header</span></span>|<span data-ttu-id="c7dc8-128">Valor</span><span class="sxs-lookup"><span data-stu-id="c7dc8-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7dc8-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7dc8-129">Authorization</span></span>|<span data-ttu-id="c7dc8-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7dc8-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7dc8-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7dc8-131">Accept</span></span>|<span data-ttu-id="c7dc8-132">application/json</span><span class="sxs-lookup"><span data-stu-id="c7dc8-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7dc8-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7dc8-133">Request body</span></span>
<span data-ttu-id="c7dc8-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7dc8-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7dc8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7dc8-135">Response</span></span>
<span data-ttu-id="c7dc8-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7dc8-136">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7dc8-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7dc8-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7dc8-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7dc8-138">Request</span></span>
<span data-ttu-id="c7dc8-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7dc8-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
```

### <a name="response"></a><span data-ttu-id="c7dc8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7dc8-140">Response</span></span>
<span data-ttu-id="c7dc8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7dc8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







