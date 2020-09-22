---
title: Obter iosLobAppProvisioningConfigurationAssignment
description: Leia as propriedades e as relações do objeto iosLobAppProvisioningConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6054a4c8b7f0ef25da14bcbe6c49a6c619f98f02
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006157"
---
# <a name="get-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="625e7-103">Obter iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="625e7-103">Get iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="625e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="625e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="625e7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="625e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="625e7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="625e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="625e7-107">Leia as propriedades e as relações do objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="625e7-107">Read properties and relationships of the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="625e7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="625e7-108">Prerequisites</span></span>
<span data-ttu-id="625e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="625e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="625e7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="625e7-111">Permission type</span></span>|<span data-ttu-id="625e7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="625e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="625e7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="625e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="625e7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="625e7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="625e7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="625e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="625e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="625e7-116">Not supported.</span></span>|
|<span data-ttu-id="625e7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="625e7-117">Application</span></span>|<span data-ttu-id="625e7-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="625e7-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="625e7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="625e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="625e7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="625e7-120">Optional query parameters</span></span>
<span data-ttu-id="625e7-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="625e7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="625e7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="625e7-122">Request headers</span></span>
|<span data-ttu-id="625e7-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="625e7-123">Header</span></span>|<span data-ttu-id="625e7-124">Valor</span><span class="sxs-lookup"><span data-stu-id="625e7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="625e7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="625e7-125">Authorization</span></span>|<span data-ttu-id="625e7-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="625e7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="625e7-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="625e7-127">Accept</span></span>|<span data-ttu-id="625e7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="625e7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="625e7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="625e7-129">Request body</span></span>
<span data-ttu-id="625e7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="625e7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="625e7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="625e7-131">Response</span></span>
<span data-ttu-id="625e7-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="625e7-132">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="625e7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="625e7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="625e7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="625e7-134">Request</span></span>
<span data-ttu-id="625e7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="625e7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="625e7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="625e7-136">Response</span></span>
<span data-ttu-id="625e7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="625e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
    "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    }
  }
}
```






