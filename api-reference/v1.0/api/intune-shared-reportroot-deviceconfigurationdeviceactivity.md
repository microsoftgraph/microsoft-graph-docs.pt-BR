---
title: Função deviceConfigurationDeviceActivity
description: Metadados para o relatório de atividade do dispositivo de configuração do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b814ff6a4143b7115d9c226243ca133bc632867d
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732290"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="f99d1-103">Função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="f99d1-103">deviceConfigurationDeviceActivity function</span></span>

<span data-ttu-id="f99d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f99d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f99d1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f99d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f99d1-106">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f99d1-106">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f99d1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f99d1-107">Prerequisites</span></span>
<span data-ttu-id="f99d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f99d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f99d1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f99d1-110">Permission type</span></span>|<span data-ttu-id="f99d1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f99d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f99d1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f99d1-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f99d1-113">&nbsp;&nbsp;Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f99d1-113">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="f99d1-114">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f99d1-114">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f99d1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f99d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f99d1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f99d1-116">Not supported.</span></span>|
|<span data-ttu-id="f99d1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f99d1-117">Application</span></span>|<span data-ttu-id="f99d1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f99d1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f99d1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f99d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="f99d1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f99d1-120">Request headers</span></span>
|<span data-ttu-id="f99d1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f99d1-121">Header</span></span>|<span data-ttu-id="f99d1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f99d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f99d1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f99d1-123">Authorization</span></span>|<span data-ttu-id="f99d1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f99d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f99d1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f99d1-125">Accept</span></span>|<span data-ttu-id="f99d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f99d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f99d1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f99d1-127">Request body</span></span>
<span data-ttu-id="f99d1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f99d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f99d1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f99d1-129">Response</span></span>
<span data-ttu-id="f99d1-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f99d1-130">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f99d1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f99d1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f99d1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f99d1-132">Request</span></span>
<span data-ttu-id="f99d1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f99d1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="f99d1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f99d1-134">Response</span></span>
<span data-ttu-id="f99d1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f99d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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














