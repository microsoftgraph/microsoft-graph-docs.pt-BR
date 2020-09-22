---
title: Obter groupPolicyOperation
description: Leia as propriedades e as relações do objeto groupPolicyOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4a3cd64195d390c5cb49a8bdba1760d4b124c527
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078833"
---
# <a name="get-grouppolicyoperation"></a><span data-ttu-id="af603-103">Obter groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="af603-103">Get groupPolicyOperation</span></span>

<span data-ttu-id="af603-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af603-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af603-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="af603-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af603-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af603-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af603-107">Leia as propriedades e as relações do objeto [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="af603-107">Read properties and relationships of the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af603-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af603-108">Prerequisites</span></span>
<span data-ttu-id="af603-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af603-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af603-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af603-111">Permission type</span></span>|<span data-ttu-id="af603-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af603-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af603-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af603-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af603-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="af603-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="af603-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af603-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af603-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af603-116">Not supported.</span></span>|
|<span data-ttu-id="af603-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af603-117">Application</span></span>|<span data-ttu-id="af603-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="af603-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af603-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af603-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations/{groupPolicyOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af603-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="af603-120">Optional query parameters</span></span>
<span data-ttu-id="af603-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="af603-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af603-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af603-122">Request headers</span></span>
|<span data-ttu-id="af603-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af603-123">Header</span></span>|<span data-ttu-id="af603-124">Valor</span><span class="sxs-lookup"><span data-stu-id="af603-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af603-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="af603-125">Authorization</span></span>|<span data-ttu-id="af603-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af603-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af603-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af603-127">Accept</span></span>|<span data-ttu-id="af603-128">application/json</span><span class="sxs-lookup"><span data-stu-id="af603-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af603-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af603-129">Request body</span></span>
<span data-ttu-id="af603-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af603-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af603-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="af603-131">Response</span></span>
<span data-ttu-id="af603-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af603-132">If successful, this method returns a `200 OK` response code and [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af603-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af603-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="af603-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af603-134">Request</span></span>
<span data-ttu-id="af603-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af603-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations/{groupPolicyOperationId}
```

### <a name="response"></a><span data-ttu-id="af603-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="af603-136">Response</span></span>
<span data-ttu-id="af603-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af603-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 316

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyOperation",
    "operationType": "upload",
    "operationStatus": "inProgress",
    "statusDetails": "Status Details value",
    "id": "4d18865b-865b-4d18-5b86-184d5b86184d",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```






