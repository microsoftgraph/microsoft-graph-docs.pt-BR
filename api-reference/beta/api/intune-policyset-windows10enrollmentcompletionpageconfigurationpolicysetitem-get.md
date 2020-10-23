---
title: Obter windows10EnrollmentCompletionPageConfigurationPolicySetItem
description: Leia as propriedades e as relações do objeto windows10EnrollmentCompletionPageConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7483929673976607e15ec76a4cf3864353cfbef6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732074"
---
# <a name="get-windows10enrollmentcompletionpageconfigurationpolicysetitem"></a><span data-ttu-id="0e9ab-103">Obter windows10EnrollmentCompletionPageConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="0e9ab-103">Get windows10EnrollmentCompletionPageConfigurationPolicySetItem</span></span>

<span data-ttu-id="0e9ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e9ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e9ab-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e9ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e9ab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e9ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e9ab-107">Leia as propriedades e as relações do objeto [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="0e9ab-107">Read properties and relationships of the [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e9ab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e9ab-108">Prerequisites</span></span>
<span data-ttu-id="0e9ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e9ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e9ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e9ab-111">Permission type</span></span>|<span data-ttu-id="0e9ab-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0e9ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e9ab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e9ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e9ab-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e9ab-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0e9ab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e9ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e9ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e9ab-116">Not supported.</span></span>|
|<span data-ttu-id="0e9ab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e9ab-117">Application</span></span>|<span data-ttu-id="0e9ab-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e9ab-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e9ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e9ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e9ab-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0e9ab-120">Optional query parameters</span></span>
<span data-ttu-id="0e9ab-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0e9ab-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e9ab-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e9ab-122">Request headers</span></span>
|<span data-ttu-id="0e9ab-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e9ab-123">Header</span></span>|<span data-ttu-id="0e9ab-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0e9ab-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e9ab-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e9ab-125">Authorization</span></span>|<span data-ttu-id="0e9ab-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e9ab-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e9ab-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e9ab-127">Accept</span></span>|<span data-ttu-id="0e9ab-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0e9ab-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e9ab-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e9ab-129">Request body</span></span>
<span data-ttu-id="0e9ab-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e9ab-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e9ab-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e9ab-131">Response</span></span>
<span data-ttu-id="0e9ab-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e9ab-132">If successful, this method returns a `200 OK` response code and [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e9ab-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e9ab-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e9ab-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e9ab-134">Request</span></span>
<span data-ttu-id="0e9ab-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e9ab-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="0e9ab-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e9ab-136">Response</span></span>
<span data-ttu-id="0e9ab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e9ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





