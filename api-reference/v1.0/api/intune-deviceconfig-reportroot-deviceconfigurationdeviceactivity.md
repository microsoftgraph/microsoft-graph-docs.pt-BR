---
title: Função deviceConfigurationDeviceActivity
description: Metadados para o relatório de atividade do dispositivo de configuração do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 036c21514e0833182e2957cf78cb2f98cbbf253e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760735"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="49c55-103">Função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="49c55-103">deviceConfigurationDeviceActivity function</span></span>

<span data-ttu-id="49c55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49c55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49c55-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49c55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49c55-106">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="49c55-106">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49c55-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49c55-107">Prerequisites</span></span>
<span data-ttu-id="49c55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49c55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49c55-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49c55-110">Permission type</span></span>|<span data-ttu-id="49c55-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49c55-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49c55-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49c55-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49c55-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="49c55-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="49c55-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49c55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49c55-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49c55-115">Not supported.</span></span>|
|<span data-ttu-id="49c55-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49c55-116">Application</span></span>|<span data-ttu-id="49c55-117">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="49c55-117">DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49c55-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49c55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="49c55-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49c55-119">Request headers</span></span>
|<span data-ttu-id="49c55-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49c55-120">Header</span></span>|<span data-ttu-id="49c55-121">Valor</span><span class="sxs-lookup"><span data-stu-id="49c55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49c55-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="49c55-122">Authorization</span></span>|<span data-ttu-id="49c55-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49c55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49c55-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49c55-124">Accept</span></span>|<span data-ttu-id="49c55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49c55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49c55-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49c55-126">Request body</span></span>
<span data-ttu-id="49c55-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49c55-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49c55-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="49c55-128">Response</span></span>
<span data-ttu-id="49c55-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-deviceconfig-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49c55-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-deviceconfig-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49c55-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49c55-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="49c55-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49c55-131">Request</span></span>
<span data-ttu-id="49c55-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49c55-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="49c55-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="49c55-133">Response</span></span>
<span data-ttu-id="49c55-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49c55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "Y29udGVudCBJbnR1bmUgRG9jIFNhbXBsZSAxNTYxOTcwNjY1"
  }
}
```




