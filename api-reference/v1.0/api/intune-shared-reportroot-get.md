---
title: Get reportRoot
description: Ler propriedades e relações do objeto reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e24a86c1ff4443b0d2867dc9f7da7e273a3012e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576801"
---
# <a name="get-reportroot"></a><span data-ttu-id="51721-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="51721-103">Get reportRoot</span></span>

> <span data-ttu-id="51721-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51721-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51721-105">Ler propriedades e relações do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="51721-105">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51721-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51721-106">Prerequisites</span></span>
<span data-ttu-id="51721-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51721-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51721-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51721-109">Permission type</span></span>|<span data-ttu-id="51721-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51721-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51721-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51721-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="51721-112">&nbsp;&nbsp; Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="51721-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="51721-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="51721-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="51721-114">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="51721-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="51721-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="51721-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="51721-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51721-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51721-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51721-117">Not supported.</span></span>|
|<span data-ttu-id="51721-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51721-118">Application</span></span>|<span data-ttu-id="51721-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51721-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51721-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51721-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51721-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="51721-121">Optional query parameters</span></span>
<span data-ttu-id="51721-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="51721-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51721-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51721-123">Request headers</span></span>
|<span data-ttu-id="51721-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51721-124">Header</span></span>|<span data-ttu-id="51721-125">Valor</span><span class="sxs-lookup"><span data-stu-id="51721-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51721-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="51721-126">Authorization</span></span>|<span data-ttu-id="51721-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51721-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51721-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51721-128">Accept</span></span>|<span data-ttu-id="51721-129">application/json</span><span class="sxs-lookup"><span data-stu-id="51721-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51721-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51721-130">Request body</span></span>
<span data-ttu-id="51721-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51721-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51721-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="51721-132">Response</span></span>
<span data-ttu-id="51721-133">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51721-133">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51721-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51721-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="51721-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51721-135">Request</span></span>
<span data-ttu-id="51721-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51721-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="51721-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="51721-137">Response</span></span>
<span data-ttu-id="51721-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51721-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








