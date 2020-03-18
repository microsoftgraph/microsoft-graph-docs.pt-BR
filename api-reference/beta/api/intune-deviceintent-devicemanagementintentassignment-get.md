---
title: Obter deviceManagementIntentAssignment
description: Leia as propriedades e as relações do objeto deviceManagementIntentAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ff084649d4c37e8f4155cb51d7ade7451fc9578
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767495"
---
# <a name="get-devicemanagementintentassignment"></a><span data-ttu-id="c5e26-103">Obter deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="c5e26-103">Get deviceManagementIntentAssignment</span></span>

> <span data-ttu-id="c5e26-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5e26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5e26-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5e26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5e26-106">Leia as propriedades e as relações do objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c5e26-106">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5e26-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5e26-107">Prerequisites</span></span>
<span data-ttu-id="c5e26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5e26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5e26-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5e26-110">Permission type</span></span>|<span data-ttu-id="c5e26-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5e26-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5e26-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5e26-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5e26-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5e26-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c5e26-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5e26-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5e26-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5e26-115">Not supported.</span></span>|
|<span data-ttu-id="c5e26-116">Application</span><span class="sxs-lookup"><span data-stu-id="c5e26-116">Application</span></span>|<span data-ttu-id="c5e26-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5e26-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5e26-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5e26-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5e26-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5e26-119">Optional query parameters</span></span>
<span data-ttu-id="c5e26-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5e26-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5e26-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5e26-121">Request headers</span></span>
|<span data-ttu-id="c5e26-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5e26-122">Header</span></span>|<span data-ttu-id="c5e26-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c5e26-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5e26-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5e26-124">Authorization</span></span>|<span data-ttu-id="c5e26-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5e26-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5e26-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5e26-126">Accept</span></span>|<span data-ttu-id="c5e26-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c5e26-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5e26-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5e26-128">Request body</span></span>
<span data-ttu-id="c5e26-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5e26-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5e26-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5e26-130">Response</span></span>
<span data-ttu-id="c5e26-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5e26-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5e26-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5e26-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5e26-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5e26-133">Request</span></span>
<span data-ttu-id="c5e26-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5e26-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c5e26-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5e26-135">Response</span></span>
<span data-ttu-id="c5e26-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5e26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
    "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




