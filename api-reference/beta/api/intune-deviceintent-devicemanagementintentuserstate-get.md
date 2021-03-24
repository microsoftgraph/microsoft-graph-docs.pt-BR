---
title: Obter deviceManagementIntentUserState
description: Ler propriedades e relações do objeto deviceManagementIntentUserState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 939a54cb7f07cfd8893f59b3f1d672e40aa761b6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130865"
---
# <a name="get-devicemanagementintentuserstate"></a><span data-ttu-id="deaae-103">Obter deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="deaae-103">Get deviceManagementIntentUserState</span></span>

<span data-ttu-id="deaae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deaae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="deaae-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="deaae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="deaae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="deaae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="deaae-107">Ler propriedades e relações do [objeto deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)</span><span class="sxs-lookup"><span data-stu-id="deaae-107">Read properties and relationships of the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="deaae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="deaae-108">Prerequisites</span></span>
<span data-ttu-id="deaae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deaae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deaae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="deaae-111">Permission type</span></span>|<span data-ttu-id="deaae-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="deaae-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="deaae-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="deaae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="deaae-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deaae-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="deaae-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="deaae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="deaae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="deaae-116">Not supported.</span></span>|
|<span data-ttu-id="deaae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="deaae-117">Application</span></span>|<span data-ttu-id="deaae-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deaae-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="deaae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="deaae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="deaae-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="deaae-120">Optional query parameters</span></span>
<span data-ttu-id="deaae-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="deaae-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="deaae-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="deaae-122">Request headers</span></span>
|<span data-ttu-id="deaae-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="deaae-123">Header</span></span>|<span data-ttu-id="deaae-124">Valor</span><span class="sxs-lookup"><span data-stu-id="deaae-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="deaae-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="deaae-125">Authorization</span></span>|<span data-ttu-id="deaae-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="deaae-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="deaae-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="deaae-127">Accept</span></span>|<span data-ttu-id="deaae-128">application/json</span><span class="sxs-lookup"><span data-stu-id="deaae-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="deaae-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="deaae-129">Request body</span></span>
<span data-ttu-id="deaae-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="deaae-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deaae-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="deaae-131">Response</span></span>
<span data-ttu-id="deaae-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="deaae-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="deaae-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="deaae-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="deaae-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="deaae-134">Request</span></span>
<span data-ttu-id="deaae-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="deaae-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

### <a name="response"></a><span data-ttu-id="deaae-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="deaae-136">Response</span></span>
<span data-ttu-id="deaae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="deaae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 357

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
    "id": "0201286a-286a-0201-6a28-01026a280102",
    "userPrincipalName": "User Principal Name value",
    "userName": "User Name value",
    "deviceCount": 11,
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "state": "notApplicable"
  }
}
```




