---
title: Função deviceConfigurationDeviceActivity
description: Metadados para o relatório de atividade do dispositivo de configuração do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 55be9ee8ffa1cd2b7dba5e91fe31df7b0f3b58f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023423"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="a483a-103">Função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="a483a-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="a483a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a483a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a483a-105">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a483a-105">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a483a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a483a-106">Prerequisites</span></span>
<span data-ttu-id="a483a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a483a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a483a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a483a-109">Permission type</span></span>|<span data-ttu-id="a483a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a483a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a483a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a483a-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a483a-112">&nbsp;&nbsp; Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a483a-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="a483a-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a483a-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a483a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a483a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a483a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a483a-115">Not supported.</span></span>|
|<span data-ttu-id="a483a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a483a-116">Application</span></span>|<span data-ttu-id="a483a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a483a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a483a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a483a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="a483a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a483a-119">Request headers</span></span>
|<span data-ttu-id="a483a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a483a-120">Header</span></span>|<span data-ttu-id="a483a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a483a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a483a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a483a-122">Authorization</span></span>|<span data-ttu-id="a483a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a483a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a483a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a483a-124">Accept</span></span>|<span data-ttu-id="a483a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a483a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a483a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a483a-126">Request body</span></span>
<span data-ttu-id="a483a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a483a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a483a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a483a-128">Response</span></span>
<span data-ttu-id="a483a-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a483a-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a483a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a483a-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="a483a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a483a-131">Request</span></span>
<span data-ttu-id="a483a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a483a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="a483a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a483a-133">Response</span></span>
<span data-ttu-id="a483a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a483a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








