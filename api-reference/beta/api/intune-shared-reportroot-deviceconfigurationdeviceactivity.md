---
title: Função deviceConfigurationDeviceActivity
description: Metadados para o relatório de atividade do dispositivo de configuração do dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f215748ff5b694e493a1bc01403e69e52951b642
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800715"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="2f82c-103">Função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="2f82c-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="2f82c-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2f82c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f82c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2f82c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f82c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f82c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f82c-107">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2f82c-107">Metadata for the device configuration device activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f82c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f82c-108">Prerequisites</span></span>
<span data-ttu-id="2f82c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f82c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f82c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f82c-111">Permission type</span></span>|<span data-ttu-id="2f82c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f82c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f82c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f82c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2f82c-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="2f82c-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2f82c-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f82c-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2f82c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f82c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f82c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f82c-117">Not supported.</span></span>|
|<span data-ttu-id="2f82c-118">Application</span><span class="sxs-lookup"><span data-stu-id="2f82c-118">Application</span></span>||
| <span data-ttu-id="2f82c-119">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="2f82c-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2f82c-120">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f82c-120">DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f82c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f82c-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="2f82c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f82c-122">Request headers</span></span>
|<span data-ttu-id="2f82c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f82c-123">Header</span></span>|<span data-ttu-id="2f82c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2f82c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f82c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f82c-125">Authorization</span></span>|<span data-ttu-id="2f82c-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f82c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f82c-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f82c-127">Accept</span></span>|<span data-ttu-id="2f82c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2f82c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f82c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f82c-129">Request body</span></span>
<span data-ttu-id="2f82c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f82c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f82c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f82c-131">Response</span></span>
<span data-ttu-id="2f82c-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f82c-132">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f82c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f82c-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f82c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f82c-134">Request</span></span>
<span data-ttu-id="2f82c-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f82c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="2f82c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f82c-136">Response</span></span>
<span data-ttu-id="2f82c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f82c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










