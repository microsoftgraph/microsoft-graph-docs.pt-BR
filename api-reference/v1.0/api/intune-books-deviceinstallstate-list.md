---
title: Listar deviceInstallStates
description: Listar propriedades e relações dos objetos deviceInstallState.
author: tfitzmac
ms.openlocfilehash: 94c4039e2605ab6139623cfac50343aac5b0b925
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350782"
---
# <a name="list-deviceinstallstates"></a><span data-ttu-id="3b462-103">Listar deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="3b462-103">List deviceInstallStates</span></span>

> <span data-ttu-id="3b462-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3b462-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b462-105">Listar propriedades e relações dos objetos [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="3b462-105">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b462-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b462-106">Prerequisites</span></span>
<span data-ttu-id="3b462-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b462-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b462-109">Permission type</span></span>|<span data-ttu-id="3b462-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b462-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b462-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b462-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b462-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b462-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3b462-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b462-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b462-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b462-114">Not supported.</span></span>|
|<span data-ttu-id="3b462-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b462-115">Application</span></span>|<span data-ttu-id="3b462-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b462-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b462-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b462-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="3b462-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b462-118">Request headers</span></span>
|<span data-ttu-id="3b462-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b462-119">Header</span></span>|<span data-ttu-id="3b462-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3b462-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b462-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b462-121">Authorization</span></span>|<span data-ttu-id="3b462-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b462-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b462-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3b462-123">Accept</span></span>|<span data-ttu-id="3b462-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3b462-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b462-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b462-125">Request body</span></span>
<span data-ttu-id="3b462-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b462-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b462-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b462-127">Response</span></span>
<span data-ttu-id="3b462-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceInstallState](../resources/intune-books-deviceinstallstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b462-128">If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b462-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b462-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b462-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b462-130">Request</span></span>
<span data-ttu-id="3b462-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b462-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="3b462-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b462-132">Response</span></span>
<span data-ttu-id="3b462-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b462-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceInstallState",
      "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "installState": "installed",
      "errorCode": "Error Code value",
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "userName": "User Name value"
    }
  ]
}
```



