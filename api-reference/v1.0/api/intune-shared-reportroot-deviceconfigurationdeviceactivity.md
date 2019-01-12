---
title: Função deviceConfigurationDeviceActivity
description: Metadados para o relatório de atividade do dispositivo de configuração do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4de84b71ba5d2e900d54c02fba965fd28e07c00a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925522"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="47546-103">Função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="47546-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="47546-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="47546-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47546-105">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="47546-105">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47546-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47546-106">Prerequisites</span></span>
<span data-ttu-id="47546-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47546-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47546-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47546-109">Permission type</span></span>|<span data-ttu-id="47546-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47546-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47546-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47546-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="47546-112">&nbsp;&nbsp; Configuração de dispositivo</span><span class="sxs-lookup"><span data-stu-id="47546-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="47546-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="47546-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="47546-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47546-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47546-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47546-115">Not supported.</span></span>|
|<span data-ttu-id="47546-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47546-116">Application</span></span>|<span data-ttu-id="47546-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47546-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47546-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47546-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="47546-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47546-119">Request headers</span></span>
|<span data-ttu-id="47546-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47546-120">Header</span></span>|<span data-ttu-id="47546-121">Valor</span><span class="sxs-lookup"><span data-stu-id="47546-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47546-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="47546-122">Authorization</span></span>|<span data-ttu-id="47546-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47546-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47546-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47546-124">Accept</span></span>|<span data-ttu-id="47546-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47546-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47546-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47546-126">Request body</span></span>
<span data-ttu-id="47546-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47546-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47546-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="47546-128">Response</span></span>
<span data-ttu-id="47546-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47546-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47546-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47546-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="47546-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47546-131">Request</span></span>
<span data-ttu-id="47546-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47546-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="47546-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="47546-133">Response</span></span>
<span data-ttu-id="47546-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47546-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```








