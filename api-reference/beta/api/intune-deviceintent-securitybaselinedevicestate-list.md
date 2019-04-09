---
title: Listar securityBaselineDeviceStates
description: Listar Propriedades e relações dos objetos securityBaselineDeviceState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 792c81187dfb5fb9388ba49e24e793adc1805b97
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522920"
---
# <a name="list-securitybaselinedevicestates"></a><span data-ttu-id="dbefd-103">Listar securityBaselineDeviceStates</span><span class="sxs-lookup"><span data-stu-id="dbefd-103">List securityBaselineDeviceStates</span></span>

> <span data-ttu-id="dbefd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dbefd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbefd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dbefd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbefd-106">Listar Propriedades e relações dos objetos [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="dbefd-106">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbefd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dbefd-107">Prerequisites</span></span>
<span data-ttu-id="dbefd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbefd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbefd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbefd-110">Permission type</span></span>|<span data-ttu-id="dbefd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dbefd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbefd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbefd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dbefd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbefd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dbefd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbefd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbefd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbefd-115">Not supported.</span></span>|
|<span data-ttu-id="dbefd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbefd-116">Application</span></span>|<span data-ttu-id="dbefd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbefd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbefd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbefd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="dbefd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbefd-119">Request headers</span></span>
|<span data-ttu-id="dbefd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbefd-120">Header</span></span>|<span data-ttu-id="dbefd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dbefd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbefd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbefd-122">Authorization</span></span>|<span data-ttu-id="dbefd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbefd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbefd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dbefd-124">Accept</span></span>|<span data-ttu-id="dbefd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dbefd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbefd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbefd-126">Request body</span></span>
<span data-ttu-id="dbefd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dbefd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbefd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbefd-128">Response</span></span>
<span data-ttu-id="dbefd-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbefd-129">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbefd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbefd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbefd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbefd-131">Request</span></span>
<span data-ttu-id="dbefd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbefd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

### <a name="response"></a><span data-ttu-id="dbefd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbefd-133">Response</span></span>
<span data-ttu-id="dbefd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbefd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 420

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
      "id": "182749bf-49bf-1827-bf49-2718bf492718",
      "managedDeviceId": "Managed Device Id value",
      "deviceDisplayName": "Device Display Name value",
      "userPrincipalName": "User Principal Name value",
      "state": "secure",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
    }
  ]
}
```







