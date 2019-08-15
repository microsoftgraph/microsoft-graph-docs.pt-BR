---
title: Obter officeClientConfigurationAssignment
description: Leia as propriedades e as relações do objeto officeClientConfigurationAssignment.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8248b1e5026d4bd9be561faa76e74e052cf9a3cb
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420830"
---
# <a name="get-officeclientconfigurationassignment"></a><span data-ttu-id="e0c39-103">Obter officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e0c39-103">Get officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="e0c39-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0c39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0c39-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0c39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0c39-106">Leia as propriedades e as relações do objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e0c39-106">Read properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0c39-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0c39-107">Prerequisites</span></span>
<span data-ttu-id="e0c39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0c39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0c39-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0c39-110">Permission type</span></span>|<span data-ttu-id="e0c39-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e0c39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0c39-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0c39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0c39-113">**TODO: Determine os escopos**</span><span class="sxs-lookup"><span data-stu-id="e0c39-113">**TODO: Determine scopes**</span></span>|
|<span data-ttu-id="e0c39-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0c39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0c39-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0c39-115">Not supported.</span></span>|
|<span data-ttu-id="e0c39-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0c39-116">Application</span></span>|<span data-ttu-id="e0c39-117">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="e0c39-117">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0c39-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0c39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0c39-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0c39-119">Optional query parameters</span></span>
<span data-ttu-id="e0c39-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0c39-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0c39-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c39-121">Request headers</span></span>
|<span data-ttu-id="e0c39-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0c39-122">Header</span></span>|<span data-ttu-id="e0c39-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e0c39-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0c39-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0c39-124">Authorization</span></span>|<span data-ttu-id="e0c39-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0c39-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0c39-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0c39-126">Accept</span></span>|<span data-ttu-id="e0c39-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e0c39-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0c39-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c39-128">Request body</span></span>
<span data-ttu-id="e0c39-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0c39-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0c39-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0c39-130">Response</span></span>
<span data-ttu-id="e0c39-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0c39-131">If successful, this method returns a `200 OK` response code and [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0c39-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0c39-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0c39-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c39-133">Request</span></span>
<span data-ttu-id="e0c39-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0c39-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e0c39-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0c39-135">Response</span></span>
<span data-ttu-id="e0c39-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0c39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
    "id": "804730f3-30f3-8047-f330-4780f3304780",
    "target": {
      "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
    }
  }
}
```






