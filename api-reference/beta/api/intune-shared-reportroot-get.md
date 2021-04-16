---
title: Get reportRoot
description: Ler propriedades e relações do objeto reportRoot.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e9c1e248ef9e6a8803f63c78656e57977ee20f43
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865422"
---
# <a name="get-reportroot"></a><span data-ttu-id="d4621-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="d4621-103">Get reportRoot</span></span>

<span data-ttu-id="d4621-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4621-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4621-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d4621-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4621-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d4621-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4621-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4621-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4621-108">Ler propriedades e relações do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d4621-108">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4621-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4621-109">Prerequisites</span></span>
<span data-ttu-id="d4621-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4621-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4621-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4621-112">Permission type</span></span>|<span data-ttu-id="d4621-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4621-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4621-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4621-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d4621-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d4621-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d4621-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4621-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d4621-117">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="d4621-117">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d4621-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4621-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d4621-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4621-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4621-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4621-120">Not supported.</span></span>|
|<span data-ttu-id="d4621-121">Application</span><span class="sxs-lookup"><span data-stu-id="d4621-121">Application</span></span>||
| <span data-ttu-id="d4621-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d4621-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d4621-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4621-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d4621-124">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="d4621-124">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d4621-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4621-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4621-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4621-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4621-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d4621-127">Optional query parameters</span></span>
<span data-ttu-id="d4621-128">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d4621-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d4621-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4621-129">Request headers</span></span>
|<span data-ttu-id="d4621-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4621-130">Header</span></span>|<span data-ttu-id="d4621-131">Valor</span><span class="sxs-lookup"><span data-stu-id="d4621-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4621-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4621-132">Authorization</span></span>|<span data-ttu-id="d4621-133">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4621-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4621-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4621-134">Accept</span></span>|<span data-ttu-id="d4621-135">application/json</span><span class="sxs-lookup"><span data-stu-id="d4621-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4621-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4621-136">Request body</span></span>
<span data-ttu-id="d4621-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4621-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4621-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4621-138">Response</span></span>
<span data-ttu-id="d4621-139">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4621-139">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4621-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4621-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4621-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4621-141">Request</span></span>
<span data-ttu-id="d4621-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4621-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="d4621-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4621-143">Response</span></span>
<span data-ttu-id="d4621-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4621-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










