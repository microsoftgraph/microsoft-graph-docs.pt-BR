---
title: Obter enrollmentRestrictionsConfigurationPolicySetItem
description: Leia as propriedades e as relações do objeto enrollmentRestrictionsConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d82a03a0c9e949d123b3e93bb64f365cc520b148
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49233121"
---
# <a name="get-enrollmentrestrictionsconfigurationpolicysetitem"></a><span data-ttu-id="13883-103">Obter enrollmentRestrictionsConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="13883-103">Get enrollmentRestrictionsConfigurationPolicySetItem</span></span>

<span data-ttu-id="13883-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13883-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13883-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13883-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13883-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13883-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13883-107">Leia as propriedades e as relações do objeto [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="13883-107">Read properties and relationships of the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13883-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13883-108">Prerequisites</span></span>
<span data-ttu-id="13883-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13883-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13883-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13883-111">Permission type</span></span>|<span data-ttu-id="13883-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13883-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13883-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13883-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13883-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13883-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="13883-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13883-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13883-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13883-116">Not supported.</span></span>|
|<span data-ttu-id="13883-117">Application</span><span class="sxs-lookup"><span data-stu-id="13883-117">Application</span></span>|<span data-ttu-id="13883-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13883-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13883-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13883-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13883-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="13883-120">Optional query parameters</span></span>
<span data-ttu-id="13883-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="13883-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13883-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13883-122">Request headers</span></span>
|<span data-ttu-id="13883-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13883-123">Header</span></span>|<span data-ttu-id="13883-124">Valor</span><span class="sxs-lookup"><span data-stu-id="13883-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13883-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="13883-125">Authorization</span></span>|<span data-ttu-id="13883-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13883-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13883-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13883-127">Accept</span></span>|<span data-ttu-id="13883-128">application/json</span><span class="sxs-lookup"><span data-stu-id="13883-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13883-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13883-129">Request body</span></span>
<span data-ttu-id="13883-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13883-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13883-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="13883-131">Response</span></span>
<span data-ttu-id="13883-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13883-132">If successful, this method returns a `200 OK` response code and [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13883-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13883-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="13883-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13883-134">Request</span></span>
<span data-ttu-id="13883-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13883-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="13883-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="13883-136">Response</span></span>
<span data-ttu-id="13883-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13883-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
    "id": "08c4f0b1-f0b1-08c4-b1f0-c408b1f0c408",
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
    "priority": 8,
    "limit": 5
  }
}
```




