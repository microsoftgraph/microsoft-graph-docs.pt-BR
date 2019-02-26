---
title: função managedDeviceEnrollmentFailureTrends
description: Metadados para o relatório de tendências de falha de inscrição
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f5374e608f5619dbbab6883a55d51da5a69e1f4b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151251"
---
# <a name="manageddeviceenrollmentfailuretrends-function"></a><span data-ttu-id="5e7cc-103">função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="5e7cc-103">managedDeviceEnrollmentFailureTrends function</span></span>

> <span data-ttu-id="5e7cc-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5e7cc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5e7cc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5e7cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e7cc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e7cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e7cc-107">Metadados para o relatório de tendências de falha de inscrição</span><span class="sxs-lookup"><span data-stu-id="5e7cc-107">Metadata for the enrollment failure trends report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e7cc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e7cc-108">Prerequisites</span></span>
<span data-ttu-id="5e7cc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e7cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="5e7cc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e7cc-111">Permission type</span></span>|<span data-ttu-id="5e7cc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e7cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e7cc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e7cc-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5e7cc-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="5e7cc-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="5e7cc-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e7cc-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5e7cc-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e7cc-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e7cc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e7cc-117">Not supported.</span></span>|
|<span data-ttu-id="5e7cc-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e7cc-118">Application</span></span>|<span data-ttu-id="5e7cc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e7cc-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e7cc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e7cc-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureTrends
```

## <a name="request-headers"></a><span data-ttu-id="5e7cc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e7cc-121">Request headers</span></span>
|<span data-ttu-id="5e7cc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e7cc-122">Header</span></span>|<span data-ttu-id="5e7cc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5e7cc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e7cc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e7cc-124">Authorization</span></span>|<span data-ttu-id="5e7cc-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e7cc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e7cc-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e7cc-126">Accept</span></span>|<span data-ttu-id="5e7cc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5e7cc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e7cc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e7cc-128">Request body</span></span>
<span data-ttu-id="5e7cc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e7cc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e7cc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e7cc-130">Response</span></span>
<span data-ttu-id="5e7cc-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e7cc-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e7cc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e7cc-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e7cc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e7cc-133">Request</span></span>
<span data-ttu-id="5e7cc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e7cc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureTrends
```

### <a name="response"></a><span data-ttu-id="5e7cc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e7cc-135">Response</span></span>
<span data-ttu-id="5e7cc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e7cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



