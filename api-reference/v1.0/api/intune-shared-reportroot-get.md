---
title: Get reportRoot
description: Ler propriedades e relações do objeto reportRoot.
ms.openlocfilehash: 5c23cc4ff2a22077f3298846af1773417cd33c28
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006743"
---
# <a name="get-reportroot"></a><span data-ttu-id="b20b7-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="b20b7-103">Get reportRoot</span></span>

> <span data-ttu-id="b20b7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b20b7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b20b7-105">Ler propriedades e relações do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="b20b7-105">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b20b7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b20b7-106">Prerequisites</span></span>
<span data-ttu-id="b20b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b20b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b20b7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b20b7-109">Permission type</span></span>|<span data-ttu-id="b20b7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b20b7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b20b7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b20b7-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b20b7-112">&nbsp;&nbsp; Configuração de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b20b7-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="b20b7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b20b7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b20b7-114">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="b20b7-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="b20b7-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b20b7-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b20b7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b20b7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b20b7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b20b7-117">Not supported.</span></span>|
|<span data-ttu-id="b20b7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b20b7-118">Application</span></span>|<span data-ttu-id="b20b7-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b20b7-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b20b7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b20b7-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b20b7-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b20b7-121">Optional query parameters</span></span>
<span data-ttu-id="b20b7-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b20b7-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b20b7-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b20b7-123">Request headers</span></span>
|<span data-ttu-id="b20b7-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b20b7-124">Header</span></span>|<span data-ttu-id="b20b7-125">Valor</span><span class="sxs-lookup"><span data-stu-id="b20b7-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b20b7-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b20b7-126">Authorization</span></span>|<span data-ttu-id="b20b7-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b20b7-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b20b7-128">Accept</span><span class="sxs-lookup"><span data-stu-id="b20b7-128">Accept</span></span>|<span data-ttu-id="b20b7-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b20b7-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b20b7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b20b7-130">Request body</span></span>
<span data-ttu-id="b20b7-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b20b7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b20b7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b20b7-132">Response</span></span>
<span data-ttu-id="b20b7-133">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b20b7-133">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b20b7-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b20b7-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="b20b7-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b20b7-135">Request</span></span>
<span data-ttu-id="b20b7-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b20b7-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="b20b7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b20b7-137">Response</span></span>
<span data-ttu-id="b20b7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b20b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```








