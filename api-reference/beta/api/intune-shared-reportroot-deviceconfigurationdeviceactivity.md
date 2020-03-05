---
title: Função deviceConfigurationDeviceActivity
description: Metadados para o relatório de atividade do dispositivo de configuração do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 68ea1e7e8eeacf7b7582bedbb65ffd27515e1967
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458214"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="69c58-103">Função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="69c58-103">deviceConfigurationDeviceActivity function</span></span>

<span data-ttu-id="69c58-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="69c58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69c58-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="69c58-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="69c58-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="69c58-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69c58-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69c58-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69c58-108">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="69c58-108">Metadata for the device configuration device activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69c58-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69c58-109">Prerequisites</span></span>
<span data-ttu-id="69c58-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69c58-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69c58-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69c58-112">Permission type</span></span>|<span data-ttu-id="69c58-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69c58-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69c58-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69c58-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="69c58-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="69c58-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="69c58-116">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69c58-116">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="69c58-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69c58-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69c58-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69c58-118">Not supported.</span></span>|
|<span data-ttu-id="69c58-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69c58-119">Application</span></span>||
| <span data-ttu-id="69c58-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="69c58-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="69c58-121">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69c58-121">DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69c58-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69c58-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="69c58-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69c58-123">Request headers</span></span>
|<span data-ttu-id="69c58-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69c58-124">Header</span></span>|<span data-ttu-id="69c58-125">Valor</span><span class="sxs-lookup"><span data-stu-id="69c58-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69c58-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="69c58-126">Authorization</span></span>|<span data-ttu-id="69c58-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69c58-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69c58-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69c58-128">Accept</span></span>|<span data-ttu-id="69c58-129">application/json</span><span class="sxs-lookup"><span data-stu-id="69c58-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69c58-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69c58-130">Request body</span></span>
<span data-ttu-id="69c58-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69c58-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69c58-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="69c58-132">Response</span></span>
<span data-ttu-id="69c58-133">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69c58-133">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69c58-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69c58-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="69c58-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69c58-135">Request</span></span>
<span data-ttu-id="69c58-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69c58-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="69c58-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="69c58-137">Response</span></span>
<span data-ttu-id="69c58-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69c58-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











