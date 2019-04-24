---
title: Listar securityBaselineStates
description: Listar Propriedades e relações dos objetos securityBaselineState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d1c334b5f377d4fd31e2209bf6940fc2bf65a76
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466109"
---
# <a name="list-securitybaselinestates"></a><span data-ttu-id="2c369-103">Listar securityBaselineStates</span><span class="sxs-lookup"><span data-stu-id="2c369-103">List securityBaselineStates</span></span>

> <span data-ttu-id="2c369-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2c369-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c369-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c369-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c369-106">Listar Propriedades e relações dos objetos [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) .</span><span class="sxs-lookup"><span data-stu-id="2c369-106">List properties and relationships of the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c369-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2c369-107">Prerequisites</span></span>
<span data-ttu-id="2c369-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c369-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c369-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c369-110">Permission type</span></span>|<span data-ttu-id="2c369-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2c369-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c369-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c369-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c369-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c369-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2c369-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c369-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c369-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c369-115">Not supported.</span></span>|
|<span data-ttu-id="2c369-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c369-116">Application</span></span>|<span data-ttu-id="2c369-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c369-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c369-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c369-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
```

## <a name="request-headers"></a><span data-ttu-id="2c369-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c369-119">Request headers</span></span>
|<span data-ttu-id="2c369-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c369-120">Header</span></span>|<span data-ttu-id="2c369-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2c369-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c369-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c369-122">Authorization</span></span>|<span data-ttu-id="2c369-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c369-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c369-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2c369-124">Accept</span></span>|<span data-ttu-id="2c369-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c369-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c369-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c369-126">Request body</span></span>
<span data-ttu-id="2c369-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c369-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c369-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c369-128">Response</span></span>
<span data-ttu-id="2c369-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c369-129">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c369-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c369-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c369-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c369-131">Request</span></span>
<span data-ttu-id="2c369-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c369-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
```

### <a name="response"></a><span data-ttu-id="2c369-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c369-133">Response</span></span>
<span data-ttu-id="2c369-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c369-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineState",
      "id": "23dc2503-2503-23dc-0325-dc230325dc23",
      "securityBaselineTemplateId": "Security Baseline Template Id value",
      "displayName": "Display Name value"
    }
  ]
}
```



