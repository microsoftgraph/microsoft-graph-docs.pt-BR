---
title: Obter windows10EnrollmentCompletionPageConfigurationPolicySetItem
description: Leia as propriedades e as relações do objeto windows10EnrollmentCompletionPageConfigurationPolicySetItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c83742434273b6b471dc11e270ec97dd22c75b8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940837"
---
# <a name="get-windows10enrollmentcompletionpageconfigurationpolicysetitem"></a><span data-ttu-id="a8156-103">Obter windows10EnrollmentCompletionPageConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="a8156-103">Get windows10EnrollmentCompletionPageConfigurationPolicySetItem</span></span>

> <span data-ttu-id="a8156-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8156-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8156-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8156-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8156-106">Leia as propriedades e as relações do objeto [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="a8156-106">Read properties and relationships of the [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8156-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8156-107">Prerequisites</span></span>
<span data-ttu-id="a8156-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8156-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8156-110">Permission type</span></span>|<span data-ttu-id="a8156-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a8156-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8156-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8156-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8156-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8156-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a8156-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8156-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8156-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8156-115">Not supported.</span></span>|
|<span data-ttu-id="a8156-116">Application</span><span class="sxs-lookup"><span data-stu-id="a8156-116">Application</span></span>|<span data-ttu-id="a8156-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8156-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8156-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8156-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8156-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a8156-119">Optional query parameters</span></span>
<span data-ttu-id="a8156-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a8156-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8156-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8156-121">Request headers</span></span>
|<span data-ttu-id="a8156-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8156-122">Header</span></span>|<span data-ttu-id="a8156-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a8156-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8156-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8156-124">Authorization</span></span>|<span data-ttu-id="a8156-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8156-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8156-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8156-126">Accept</span></span>|<span data-ttu-id="a8156-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a8156-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8156-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8156-128">Request body</span></span>
<span data-ttu-id="a8156-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8156-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8156-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8156-130">Response</span></span>
<span data-ttu-id="a8156-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8156-131">If successful, this method returns a `200 OK` response code and [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8156-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8156-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8156-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8156-133">Request</span></span>
<span data-ttu-id="a8156-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8156-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="a8156-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8156-135">Response</span></span>
<span data-ttu-id="a8156-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8156-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfigurationPolicySetItem",
    "id": "ebfb1dbb-1dbb-ebfb-bb1d-fbebbb1dfbeb",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "payloadId": "Payload Id value",
    "itemType": "Item Type value",
    "displayName": "Display Name value",
    "status": "validating",
    "errorCode": "unauthorized",
    "guidedDeploymentTags": [
      "Guided Deployment Tags value"
    ],
    "priority": 8
  }
}
```





