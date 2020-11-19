---
title: Obter deviceCompliancePolicyPolicySetItem
description: Leia as propriedades e as relações do objeto deviceCompliancePolicyPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1008a3e08b1dd21caff37e1d29e742eb33dcc95d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49305236"
---
# <a name="get-devicecompliancepolicypolicysetitem"></a><span data-ttu-id="1c222-103">Obter deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="1c222-103">Get deviceCompliancePolicyPolicySetItem</span></span>

<span data-ttu-id="1c222-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c222-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c222-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c222-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c222-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c222-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c222-107">Leia as propriedades e as relações do objeto [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="1c222-107">Read properties and relationships of the [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c222-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c222-108">Prerequisites</span></span>
<span data-ttu-id="1c222-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c222-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c222-111">Permission type</span></span>|<span data-ttu-id="1c222-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c222-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c222-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c222-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c222-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c222-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1c222-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c222-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c222-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c222-116">Not supported.</span></span>|
|<span data-ttu-id="1c222-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c222-117">Application</span></span>|<span data-ttu-id="1c222-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c222-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c222-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c222-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c222-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c222-120">Optional query parameters</span></span>
<span data-ttu-id="1c222-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c222-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c222-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c222-122">Request headers</span></span>
|<span data-ttu-id="1c222-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c222-123">Header</span></span>|<span data-ttu-id="1c222-124">Valor</span><span class="sxs-lookup"><span data-stu-id="1c222-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c222-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c222-125">Authorization</span></span>|<span data-ttu-id="1c222-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c222-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c222-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c222-127">Accept</span></span>|<span data-ttu-id="1c222-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1c222-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c222-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c222-129">Request body</span></span>
<span data-ttu-id="1c222-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c222-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c222-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c222-131">Response</span></span>
<span data-ttu-id="1c222-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c222-132">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c222-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c222-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c222-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c222-134">Request</span></span>
<span data-ttu-id="1c222-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c222-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="1c222-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c222-136">Response</span></span>
<span data-ttu-id="1c222-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c222-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
    "id": "5c0bc827-c827-5c0b-27c8-0b5c27c80b5c",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "payloadId": "Payload Id value",
    "itemType": "Item Type value",
    "displayName": "Display Name value",
    "status": "validating",
    "errorCode": "unauthorized",
    "guidedDeploymentTags": [
      "Guided Deployment Tags value"
    ]
  }
}
```




