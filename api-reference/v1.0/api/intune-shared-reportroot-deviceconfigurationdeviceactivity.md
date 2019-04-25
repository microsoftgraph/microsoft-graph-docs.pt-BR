---
title: Função deviceConfigurationDeviceActivity
description: Metadados para o relatório de atividade do dispositivo de configuração do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a92ca929c45e9da34e598df079197fd76a2761bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576934"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="d38e0-103">Função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="d38e0-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="d38e0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d38e0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d38e0-105">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d38e0-105">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d38e0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d38e0-106">Prerequisites</span></span>
<span data-ttu-id="d38e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d38e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d38e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d38e0-109">Permission type</span></span>|<span data-ttu-id="d38e0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d38e0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d38e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d38e0-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d38e0-112">&nbsp;&nbsp; Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d38e0-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="d38e0-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d38e0-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d38e0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d38e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d38e0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d38e0-115">Not supported.</span></span>|
|<span data-ttu-id="d38e0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d38e0-116">Application</span></span>|<span data-ttu-id="d38e0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d38e0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d38e0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d38e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="d38e0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d38e0-119">Request headers</span></span>
|<span data-ttu-id="d38e0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d38e0-120">Header</span></span>|<span data-ttu-id="d38e0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d38e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d38e0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d38e0-122">Authorization</span></span>|<span data-ttu-id="d38e0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d38e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d38e0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d38e0-124">Accept</span></span>|<span data-ttu-id="d38e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d38e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d38e0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d38e0-126">Request body</span></span>
<span data-ttu-id="d38e0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d38e0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d38e0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d38e0-128">Response</span></span>
<span data-ttu-id="d38e0-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d38e0-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d38e0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d38e0-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="d38e0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d38e0-131">Request</span></span>
<span data-ttu-id="d38e0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d38e0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="d38e0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d38e0-133">Response</span></span>
<span data-ttu-id="d38e0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d38e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








