---
title: Função deviceConfigurationUserActivity
description: Metadados para o relatório de atividades do usuário de configuração do dispositivo
ms.openlocfilehash: 92a82fc79cbf7e19fa408a51e6c38adc9b32734b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004777"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="c5cbd-103">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="c5cbd-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="c5cbd-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c5cbd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5cbd-105">Metadados para o relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c5cbd-105">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5cbd-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5cbd-106">Prerequisites</span></span>
<span data-ttu-id="c5cbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5cbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5cbd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5cbd-109">Permission type</span></span>|<span data-ttu-id="c5cbd-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5cbd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5cbd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5cbd-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c5cbd-112">&nbsp;&nbsp; Configuração de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c5cbd-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="c5cbd-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5cbd-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c5cbd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5cbd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5cbd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5cbd-115">Not supported.</span></span>|
|<span data-ttu-id="c5cbd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5cbd-116">Application</span></span>|<span data-ttu-id="c5cbd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5cbd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5cbd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5cbd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="c5cbd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5cbd-119">Request headers</span></span>
|<span data-ttu-id="c5cbd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5cbd-120">Header</span></span>|<span data-ttu-id="c5cbd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c5cbd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5cbd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5cbd-122">Authorization</span></span>|<span data-ttu-id="c5cbd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5cbd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5cbd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c5cbd-124">Accept</span></span>|<span data-ttu-id="c5cbd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5cbd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5cbd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5cbd-126">Request body</span></span>
<span data-ttu-id="c5cbd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5cbd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5cbd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5cbd-128">Response</span></span>
<span data-ttu-id="c5cbd-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5cbd-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5cbd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5cbd-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5cbd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5cbd-131">Request</span></span>
<span data-ttu-id="c5cbd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5cbd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="c5cbd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5cbd-133">Response</span></span>
<span data-ttu-id="c5cbd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5cbd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








