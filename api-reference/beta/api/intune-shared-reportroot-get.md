---
title: Get reportRoot
description: Ler propriedades e relações do objeto reportRoot.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f40622bee1ac09a6e3c98870863c7c1439bbe936
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195871"
---
# <a name="get-reportroot"></a><span data-ttu-id="b6f6c-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="b6f6c-103">Get reportRoot</span></span>

> <span data-ttu-id="b6f6c-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b6f6c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6f6c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6f6c-107">Ler propriedades e relações do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="b6f6c-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6f6c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6f6c-108">Prerequisites</span></span>
<span data-ttu-id="b6f6c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6f6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6f6c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6f6c-111">Permission type</span></span>|<span data-ttu-id="b6f6c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6f6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6f6c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6f6c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b6f6c-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b6f6c-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b6f6c-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6f6c-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b6f6c-116">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="b6f6c-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b6f6c-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6f6c-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b6f6c-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6f6c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6f6c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-119">Not supported.</span></span>|
|<span data-ttu-id="b6f6c-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6f6c-120">Application</span></span>||
| <span data-ttu-id="b6f6c-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b6f6c-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b6f6c-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6f6c-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b6f6c-123">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="b6f6c-123">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b6f6c-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6f6c-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6f6c-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6f6c-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6f6c-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6f6c-126">Optional query parameters</span></span>
<span data-ttu-id="b6f6c-127">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b6f6c-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f6c-128">Request headers</span></span>
|<span data-ttu-id="b6f6c-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6f6c-129">Header</span></span>|<span data-ttu-id="b6f6c-130">Valor</span><span class="sxs-lookup"><span data-stu-id="b6f6c-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6f6c-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6f6c-131">Authorization</span></span>|<span data-ttu-id="b6f6c-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6f6c-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6f6c-133">Accept</span></span>|<span data-ttu-id="b6f6c-134">application/json</span><span class="sxs-lookup"><span data-stu-id="b6f6c-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6f6c-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f6c-135">Request body</span></span>
<span data-ttu-id="b6f6c-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6f6c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f6c-137">Response</span></span>
<span data-ttu-id="b6f6c-138">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-138">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6f6c-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6f6c-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6f6c-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f6c-140">Request</span></span>
<span data-ttu-id="b6f6c-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="b6f6c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f6c-142">Response</span></span>
<span data-ttu-id="b6f6c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







