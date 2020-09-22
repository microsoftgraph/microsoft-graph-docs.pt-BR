---
title: Get reportRoot
description: Ler propriedades e relações do objeto reportRoot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9dffd70c71578a7f0acc97f03b0e73b1a73d2ead
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053794"
---
# <a name="get-reportroot"></a><span data-ttu-id="99448-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="99448-103">Get reportRoot</span></span>

<span data-ttu-id="99448-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99448-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99448-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99448-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="99448-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99448-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99448-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99448-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99448-108">Ler propriedades e relações do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="99448-108">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="99448-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99448-109">Prerequisites</span></span>
<span data-ttu-id="99448-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99448-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99448-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99448-112">Permission type</span></span>|<span data-ttu-id="99448-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99448-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99448-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99448-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="99448-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="99448-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="99448-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="99448-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="99448-117">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="99448-117">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="99448-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="99448-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="99448-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99448-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99448-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99448-120">Not supported.</span></span>|
|<span data-ttu-id="99448-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99448-121">Application</span></span>||
| <span data-ttu-id="99448-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="99448-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="99448-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="99448-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="99448-124">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="99448-124">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="99448-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="99448-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99448-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99448-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99448-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="99448-127">Optional query parameters</span></span>
<span data-ttu-id="99448-128">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="99448-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="99448-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99448-129">Request headers</span></span>
|<span data-ttu-id="99448-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99448-130">Header</span></span>|<span data-ttu-id="99448-131">Valor</span><span class="sxs-lookup"><span data-stu-id="99448-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99448-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="99448-132">Authorization</span></span>|<span data-ttu-id="99448-133">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99448-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99448-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99448-134">Accept</span></span>|<span data-ttu-id="99448-135">application/json</span><span class="sxs-lookup"><span data-stu-id="99448-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99448-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99448-136">Request body</span></span>
<span data-ttu-id="99448-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99448-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99448-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="99448-138">Response</span></span>
<span data-ttu-id="99448-139">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99448-139">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99448-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99448-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="99448-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99448-141">Request</span></span>
<span data-ttu-id="99448-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99448-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="99448-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="99448-143">Response</span></span>
<span data-ttu-id="99448-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99448-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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












