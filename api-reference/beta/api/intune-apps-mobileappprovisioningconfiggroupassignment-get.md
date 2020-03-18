---
title: Obter mobileAppProvisioningConfigGroupAssignment
description: Leia as propriedades e as relações do objeto mobileAppProvisioningConfigGroupAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5becc58429e118ab1c4c66d0328ff9ef79603800
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761171"
---
# <a name="get-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="a2eb2-103">Obter mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a2eb2-103">Get mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="a2eb2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2eb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2eb2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2eb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2eb2-106">Leia as propriedades e as relações do objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a2eb2-106">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2eb2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2eb2-107">Prerequisites</span></span>
<span data-ttu-id="a2eb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2eb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2eb2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2eb2-110">Permission type</span></span>|<span data-ttu-id="a2eb2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2eb2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2eb2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2eb2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2eb2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2eb2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a2eb2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2eb2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2eb2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2eb2-115">Not supported.</span></span>|
|<span data-ttu-id="a2eb2-116">Application</span><span class="sxs-lookup"><span data-stu-id="a2eb2-116">Application</span></span>|<span data-ttu-id="a2eb2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2eb2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2eb2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2eb2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2eb2-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a2eb2-119">Optional query parameters</span></span>
<span data-ttu-id="a2eb2-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a2eb2-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2eb2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2eb2-121">Request headers</span></span>
|<span data-ttu-id="a2eb2-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2eb2-122">Header</span></span>|<span data-ttu-id="a2eb2-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a2eb2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2eb2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2eb2-124">Authorization</span></span>|<span data-ttu-id="a2eb2-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2eb2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2eb2-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2eb2-126">Accept</span></span>|<span data-ttu-id="a2eb2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a2eb2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2eb2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2eb2-128">Request body</span></span>
<span data-ttu-id="a2eb2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2eb2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2eb2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2eb2-130">Response</span></span>
<span data-ttu-id="a2eb2-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2eb2-131">If successful, this method returns a `200 OK` response code and [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2eb2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2eb2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2eb2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2eb2-133">Request</span></span>
<span data-ttu-id="a2eb2-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2eb2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="a2eb2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2eb2-135">Response</span></span>
<span data-ttu-id="a2eb2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2eb2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 203

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
    "targetGroupId": "Target Group Id value",
    "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
  }
}
```




