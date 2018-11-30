---
title: função managedDeviceEnrollmentFailureTrends
description: Metadados para o relatório de tendências de falha de inscrição
ms.openlocfilehash: bebbebfff3b37ef940e55583e859736f6caf92cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040882"
---
# <a name="manageddeviceenrollmentfailuretrends-function"></a><span data-ttu-id="fd7da-103">função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="fd7da-103">managedDeviceEnrollmentFailureTrends function</span></span>

> <span data-ttu-id="fd7da-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fd7da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd7da-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fd7da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd7da-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fd7da-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd7da-107">Metadados para o relatório de tendências de falha de inscrição</span><span class="sxs-lookup"><span data-stu-id="fd7da-107">Metadata for the enrollment failure trends report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd7da-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd7da-108">Prerequisites</span></span>
<span data-ttu-id="fd7da-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd7da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd7da-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd7da-111">Permission type</span></span>|<span data-ttu-id="fd7da-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd7da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd7da-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd7da-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fd7da-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="fd7da-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fd7da-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd7da-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fd7da-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd7da-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd7da-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd7da-117">Not supported.</span></span>|
|<span data-ttu-id="fd7da-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd7da-118">Application</span></span>|<span data-ttu-id="fd7da-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd7da-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd7da-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd7da-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureTrends
```

## <a name="request-headers"></a><span data-ttu-id="fd7da-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd7da-121">Request headers</span></span>
|<span data-ttu-id="fd7da-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd7da-122">Header</span></span>|<span data-ttu-id="fd7da-123">Valor</span><span class="sxs-lookup"><span data-stu-id="fd7da-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd7da-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd7da-124">Authorization</span></span>|<span data-ttu-id="fd7da-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd7da-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd7da-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fd7da-126">Accept</span></span>|<span data-ttu-id="fd7da-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fd7da-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd7da-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd7da-128">Request body</span></span>
<span data-ttu-id="fd7da-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fd7da-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd7da-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd7da-130">Response</span></span>
<span data-ttu-id="fd7da-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd7da-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd7da-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd7da-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd7da-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd7da-133">Request</span></span>
<span data-ttu-id="fd7da-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd7da-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureTrends
```

### <a name="response"></a><span data-ttu-id="fd7da-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd7da-135">Response</span></span>
<span data-ttu-id="fd7da-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd7da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



