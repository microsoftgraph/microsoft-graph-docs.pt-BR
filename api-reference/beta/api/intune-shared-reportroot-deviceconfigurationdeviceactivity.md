---
title: Função deviceConfigurationDeviceActivity
description: Metadados para o relatório de atividade do dispositivo de configuração do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e73b6158d54872e4cae84b18e9a2d42571efbb31
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404803"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="15a16-103">Função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="15a16-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="15a16-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="15a16-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15a16-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="15a16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15a16-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="15a16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15a16-107">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="15a16-107">Metadata for the device configuration device activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15a16-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15a16-108">Prerequisites</span></span>
<span data-ttu-id="15a16-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15a16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15a16-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15a16-111">Permission type</span></span>|<span data-ttu-id="15a16-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15a16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15a16-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15a16-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="15a16-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="15a16-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="15a16-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="15a16-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="15a16-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15a16-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15a16-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15a16-117">Not supported.</span></span>|
|<span data-ttu-id="15a16-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15a16-118">Application</span></span>|<span data-ttu-id="15a16-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15a16-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15a16-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15a16-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="15a16-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15a16-121">Request headers</span></span>
|<span data-ttu-id="15a16-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15a16-122">Header</span></span>|<span data-ttu-id="15a16-123">Valor</span><span class="sxs-lookup"><span data-stu-id="15a16-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15a16-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="15a16-124">Authorization</span></span>|<span data-ttu-id="15a16-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15a16-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15a16-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15a16-126">Accept</span></span>|<span data-ttu-id="15a16-127">application/json</span><span class="sxs-lookup"><span data-stu-id="15a16-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15a16-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15a16-128">Request body</span></span>
<span data-ttu-id="15a16-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15a16-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15a16-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="15a16-130">Response</span></span>
<span data-ttu-id="15a16-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15a16-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15a16-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15a16-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="15a16-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15a16-133">Request</span></span>
<span data-ttu-id="15a16-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15a16-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="15a16-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="15a16-135">Response</span></span>
<span data-ttu-id="15a16-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15a16-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



