---
title: Obter officeClientConfigurationAssignment
description: Leia as propriedades e as relações do objeto officeClientConfigurationAssignment.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a77552daf69df542d963ed45c84385f23283a51d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444431"
---
# <a name="get-officeclientconfigurationassignment"></a><span data-ttu-id="dcfee-103">Obter officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="dcfee-103">Get officeClientConfigurationAssignment</span></span>

<span data-ttu-id="dcfee-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dcfee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcfee-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dcfee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcfee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dcfee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcfee-107">Leia as propriedades e as relações do objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="dcfee-107">Read properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcfee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dcfee-108">Prerequisites</span></span>
<span data-ttu-id="dcfee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcfee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcfee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcfee-111">Permission type</span></span>|<span data-ttu-id="dcfee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dcfee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcfee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcfee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dcfee-114">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="dcfee-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="dcfee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcfee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcfee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcfee-116">Not supported.</span></span>|
|<span data-ttu-id="dcfee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcfee-117">Application</span></span>|<span data-ttu-id="dcfee-118">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="dcfee-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcfee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcfee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dcfee-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dcfee-120">Optional query parameters</span></span>
<span data-ttu-id="dcfee-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dcfee-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcfee-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcfee-122">Request headers</span></span>
|<span data-ttu-id="dcfee-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dcfee-123">Header</span></span>|<span data-ttu-id="dcfee-124">Valor</span><span class="sxs-lookup"><span data-stu-id="dcfee-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcfee-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcfee-125">Authorization</span></span>|<span data-ttu-id="dcfee-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcfee-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcfee-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dcfee-127">Accept</span></span>|<span data-ttu-id="dcfee-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dcfee-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcfee-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcfee-129">Request body</span></span>
<span data-ttu-id="dcfee-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dcfee-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcfee-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcfee-131">Response</span></span>
<span data-ttu-id="dcfee-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcfee-132">If successful, this method returns a `200 OK` response code and [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcfee-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dcfee-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcfee-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcfee-134">Request</span></span>
<span data-ttu-id="dcfee-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcfee-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="dcfee-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcfee-136">Response</span></span>
<span data-ttu-id="dcfee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcfee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





