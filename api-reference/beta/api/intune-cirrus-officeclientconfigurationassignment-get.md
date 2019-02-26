---
title: Obter officeClientConfigurationAssignment
description: Leia as propriedades e as relações do objeto officeClientConfigurationAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6cf3416b606fc1fa32d3657ef77317834980a046
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146687"
---
# <a name="get-officeclientconfigurationassignment"></a><span data-ttu-id="89ccd-103">Obter officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="89ccd-103">Get officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="89ccd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89ccd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89ccd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89ccd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89ccd-106">Leia as propriedades e as relações do objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="89ccd-106">Read properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89ccd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89ccd-107">Prerequisites</span></span>
<span data-ttu-id="89ccd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89ccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ccd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89ccd-110">Permission type</span></span>|<span data-ttu-id="89ccd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89ccd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89ccd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89ccd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89ccd-113">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="89ccd-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="89ccd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89ccd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89ccd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89ccd-115">Not supported.</span></span>|
|<span data-ttu-id="89ccd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89ccd-116">Application</span></span>|<span data-ttu-id="89ccd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89ccd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89ccd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89ccd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89ccd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="89ccd-119">Optional query parameters</span></span>
<span data-ttu-id="89ccd-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="89ccd-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89ccd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89ccd-121">Request headers</span></span>
|<span data-ttu-id="89ccd-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89ccd-122">Header</span></span>|<span data-ttu-id="89ccd-123">Valor</span><span class="sxs-lookup"><span data-stu-id="89ccd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89ccd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="89ccd-124">Authorization</span></span>|<span data-ttu-id="89ccd-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89ccd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89ccd-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89ccd-126">Accept</span></span>|<span data-ttu-id="89ccd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="89ccd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89ccd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89ccd-128">Request body</span></span>
<span data-ttu-id="89ccd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89ccd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89ccd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ccd-130">Response</span></span>
<span data-ttu-id="89ccd-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89ccd-131">If successful, this method returns a `200 OK` response code and [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89ccd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89ccd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="89ccd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89ccd-133">Request</span></span>
<span data-ttu-id="89ccd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89ccd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="89ccd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ccd-135">Response</span></span>
<span data-ttu-id="89ccd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89ccd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



