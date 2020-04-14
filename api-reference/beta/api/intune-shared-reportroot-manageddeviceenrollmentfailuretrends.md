---
title: função managedDeviceEnrollmentFailureTrends
description: Metadados para o relatório de tendências de falha de inscrição
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 633ac84c7c37477ebb31d7b9465e9e91a83f6cdb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470301"
---
# <a name="manageddeviceenrollmentfailuretrends-function"></a><span data-ttu-id="03537-103">função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="03537-103">managedDeviceEnrollmentFailureTrends function</span></span>

<span data-ttu-id="03537-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03537-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03537-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="03537-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="03537-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="03537-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03537-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03537-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03537-108">Metadados para o relatório de tendências de falha de inscrição</span><span class="sxs-lookup"><span data-stu-id="03537-108">Metadata for the enrollment failure trends report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03537-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03537-109">Prerequisites</span></span>
<span data-ttu-id="03537-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03537-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03537-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03537-112">Permission type</span></span>|<span data-ttu-id="03537-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03537-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03537-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03537-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="03537-115">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="03537-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="03537-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03537-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="03537-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03537-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03537-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03537-118">Not supported.</span></span>|
|<span data-ttu-id="03537-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03537-119">Application</span></span>||
| <span data-ttu-id="03537-120">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="03537-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="03537-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03537-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03537-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03537-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureTrends
```

## <a name="request-headers"></a><span data-ttu-id="03537-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03537-123">Request headers</span></span>
|<span data-ttu-id="03537-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03537-124">Header</span></span>|<span data-ttu-id="03537-125">Valor</span><span class="sxs-lookup"><span data-stu-id="03537-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03537-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="03537-126">Authorization</span></span>|<span data-ttu-id="03537-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03537-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03537-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03537-128">Accept</span></span>|<span data-ttu-id="03537-129">application/json</span><span class="sxs-lookup"><span data-stu-id="03537-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03537-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03537-130">Request body</span></span>
<span data-ttu-id="03537-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03537-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03537-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="03537-132">Response</span></span>
<span data-ttu-id="03537-133">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03537-133">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03537-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03537-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="03537-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03537-135">Request</span></span>
<span data-ttu-id="03537-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03537-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureTrends
```

### <a name="response"></a><span data-ttu-id="03537-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="03537-137">Response</span></span>
<span data-ttu-id="03537-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03537-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









