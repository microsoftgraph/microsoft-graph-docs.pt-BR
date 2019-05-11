---
title: Função deviceConfigurationDeviceActivity
description: Metadados para o relatório de atividade do dispositivo de configuração do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a200c549afcb702a4ea62138322e1b5435965837
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899035"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="da7aa-103">Função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="da7aa-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="da7aa-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da7aa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da7aa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da7aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da7aa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da7aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da7aa-107">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="da7aa-107">Metadata for the device configuration device activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da7aa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da7aa-108">Prerequisites</span></span>
<span data-ttu-id="da7aa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da7aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da7aa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da7aa-111">Permission type</span></span>|<span data-ttu-id="da7aa-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da7aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da7aa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da7aa-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="da7aa-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="da7aa-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="da7aa-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="da7aa-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="da7aa-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da7aa-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da7aa-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da7aa-117">Not supported.</span></span>|
|<span data-ttu-id="da7aa-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da7aa-118">Application</span></span>|<span data-ttu-id="da7aa-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da7aa-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da7aa-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da7aa-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="da7aa-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da7aa-121">Request headers</span></span>
|<span data-ttu-id="da7aa-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da7aa-122">Header</span></span>|<span data-ttu-id="da7aa-123">Valor</span><span class="sxs-lookup"><span data-stu-id="da7aa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da7aa-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="da7aa-124">Authorization</span></span>|<span data-ttu-id="da7aa-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da7aa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da7aa-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="da7aa-126">Accept</span></span>|<span data-ttu-id="da7aa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="da7aa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da7aa-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da7aa-128">Request body</span></span>
<span data-ttu-id="da7aa-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da7aa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da7aa-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="da7aa-130">Response</span></span>
<span data-ttu-id="da7aa-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da7aa-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da7aa-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da7aa-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="da7aa-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da7aa-133">Request</span></span>
<span data-ttu-id="da7aa-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da7aa-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="da7aa-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="da7aa-135">Response</span></span>
<span data-ttu-id="da7aa-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da7aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



