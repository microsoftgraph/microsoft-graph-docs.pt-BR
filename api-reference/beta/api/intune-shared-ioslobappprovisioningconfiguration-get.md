---
title: Obter iosLobAppProvisioningConfiguration
description: Leia as propriedades e as relações do objeto iosLobAppProvisioningConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 14d1f0ae26bfe4b91005422f47da7542991a8746
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210092"
---
# <a name="get-ioslobappprovisioningconfiguration"></a><span data-ttu-id="c50d0-103">Obter iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="c50d0-103">Get iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="c50d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c50d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c50d0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c50d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c50d0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c50d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c50d0-107">Leia as propriedades e as relações do objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c50d0-107">Read properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c50d0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c50d0-108">Prerequisites</span></span>
<span data-ttu-id="c50d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c50d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c50d0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c50d0-111">Permission type</span></span>|<span data-ttu-id="c50d0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c50d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c50d0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c50d0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c50d0-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="c50d0-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="c50d0-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c50d0-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="c50d0-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="c50d0-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c50d0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c50d0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c50d0-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c50d0-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c50d0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c50d0-119">Not supported.</span></span>|
|<span data-ttu-id="c50d0-120">Application</span><span class="sxs-lookup"><span data-stu-id="c50d0-120">Application</span></span>||
| <span data-ttu-id="c50d0-121">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="c50d0-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="c50d0-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c50d0-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="c50d0-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="c50d0-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c50d0-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c50d0-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c50d0-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c50d0-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c50d0-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c50d0-126">Optional query parameters</span></span>
<span data-ttu-id="c50d0-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c50d0-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c50d0-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c50d0-128">Request headers</span></span>
|<span data-ttu-id="c50d0-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c50d0-129">Header</span></span>|<span data-ttu-id="c50d0-130">Valor</span><span class="sxs-lookup"><span data-stu-id="c50d0-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c50d0-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="c50d0-131">Authorization</span></span>|<span data-ttu-id="c50d0-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c50d0-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c50d0-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c50d0-133">Accept</span></span>|<span data-ttu-id="c50d0-134">application/json</span><span class="sxs-lookup"><span data-stu-id="c50d0-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c50d0-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c50d0-135">Request body</span></span>
<span data-ttu-id="c50d0-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c50d0-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c50d0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c50d0-137">Response</span></span>
<span data-ttu-id="c50d0-138">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c50d0-138">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c50d0-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c50d0-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="c50d0-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c50d0-140">Request</span></span>
<span data-ttu-id="c50d0-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c50d0-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c50d0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c50d0-142">Response</span></span>
<span data-ttu-id="c50d0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c50d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "value": {
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
}
```







