---
title: Listar deviceManagementIntentUserStates
description: Listar Propriedades e relações dos objetos deviceManagementIntentUserState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2be6cdf14648768e86aef9bd9d4ef4b4d0ed812
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986746"
---
# <a name="list-devicemanagementintentuserstates"></a><span data-ttu-id="63acf-103">Listar deviceManagementIntentUserStates</span><span class="sxs-lookup"><span data-stu-id="63acf-103">List deviceManagementIntentUserStates</span></span>

<span data-ttu-id="63acf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63acf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63acf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63acf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63acf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63acf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63acf-107">Listar Propriedades e relações dos objetos [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="63acf-107">List properties and relationships of the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63acf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63acf-108">Prerequisites</span></span>
<span data-ttu-id="63acf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63acf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63acf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63acf-111">Permission type</span></span>|<span data-ttu-id="63acf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63acf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63acf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63acf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63acf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63acf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="63acf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63acf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63acf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63acf-116">Not supported.</span></span>|
|<span data-ttu-id="63acf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63acf-117">Application</span></span>|<span data-ttu-id="63acf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63acf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63acf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63acf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/userStates
```

## <a name="request-headers"></a><span data-ttu-id="63acf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63acf-120">Request headers</span></span>
|<span data-ttu-id="63acf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63acf-121">Header</span></span>|<span data-ttu-id="63acf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="63acf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63acf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="63acf-123">Authorization</span></span>|<span data-ttu-id="63acf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63acf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63acf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63acf-125">Accept</span></span>|<span data-ttu-id="63acf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63acf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63acf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63acf-127">Request body</span></span>
<span data-ttu-id="63acf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63acf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63acf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="63acf-129">Response</span></span>
<span data-ttu-id="63acf-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63acf-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63acf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63acf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="63acf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63acf-132">Request</span></span>
<span data-ttu-id="63acf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63acf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates
```

### <a name="response"></a><span data-ttu-id="63acf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="63acf-134">Response</span></span>
<span data-ttu-id="63acf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63acf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
      "id": "0201286a-286a-0201-6a28-01026a280102",
      "userPrincipalName": "User Principal Name value",
      "userName": "User Name value",
      "deviceCount": 11,
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "state": "notApplicable"
    }
  ]
}
```






