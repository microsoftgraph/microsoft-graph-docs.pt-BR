---
title: Obter embeddedSIMActivationCodePoolAssignment
description: Leia as propriedades e as relações do objeto embeddedSIMActivationCodePoolAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b4dd90607c3ddff5403aa096e7a75c54b0dd595f
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087177"
---
# <a name="get-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="37f76-103">Obter embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="37f76-103">Get embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="37f76-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37f76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37f76-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37f76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37f76-106">Leia as propriedades e as relações do objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="37f76-106">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37f76-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37f76-107">Prerequisites</span></span>
<span data-ttu-id="37f76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37f76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37f76-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37f76-110">Permission type</span></span>|<span data-ttu-id="37f76-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37f76-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37f76-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37f76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37f76-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="37f76-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="37f76-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37f76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37f76-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37f76-115">Not supported.</span></span>|
|<span data-ttu-id="37f76-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37f76-116">Application</span></span>|<span data-ttu-id="37f76-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="37f76-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37f76-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37f76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37f76-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37f76-119">Optional query parameters</span></span>
<span data-ttu-id="37f76-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="37f76-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37f76-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37f76-121">Request headers</span></span>
|<span data-ttu-id="37f76-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37f76-122">Header</span></span>|<span data-ttu-id="37f76-123">Valor</span><span class="sxs-lookup"><span data-stu-id="37f76-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37f76-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="37f76-124">Authorization</span></span>|<span data-ttu-id="37f76-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37f76-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37f76-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37f76-126">Accept</span></span>|<span data-ttu-id="37f76-127">application/json</span><span class="sxs-lookup"><span data-stu-id="37f76-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37f76-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37f76-128">Request body</span></span>
<span data-ttu-id="37f76-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37f76-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37f76-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="37f76-130">Response</span></span>
<span data-ttu-id="37f76-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37f76-131">If successful, this method returns a `200 OK` response code and [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37f76-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37f76-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="37f76-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37f76-133">Request</span></span>
<span data-ttu-id="37f76-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37f76-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

### <a name="response"></a><span data-ttu-id="37f76-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="37f76-135">Response</span></span>
<span data-ttu-id="37f76-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37f76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "value": {
    "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
    "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```






