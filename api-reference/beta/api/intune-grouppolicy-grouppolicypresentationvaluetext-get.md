---
title: Obter groupPolicyPresentationValueText
description: Leia as propriedades e as relações do objeto groupPolicyPresentationValueText.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5558d46e41132b84fa6c23b92eafc2274eb8b50
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193477"
---
# <a name="get-grouppolicypresentationvaluetext"></a><span data-ttu-id="e13e9-103">Obter groupPolicyPresentationValueText</span><span class="sxs-lookup"><span data-stu-id="e13e9-103">Get groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="e13e9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e13e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e13e9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e13e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e13e9-106">Leia as propriedades e as relações do objeto [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="e13e9-106">Read properties and relationships of the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e13e9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e13e9-107">Prerequisites</span></span>
<span data-ttu-id="e13e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e13e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e13e9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e13e9-110">Permission type</span></span>|<span data-ttu-id="e13e9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e13e9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e13e9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e13e9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e13e9-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e13e9-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e13e9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e13e9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e13e9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e13e9-115">Not supported.</span></span>|
|<span data-ttu-id="e13e9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e13e9-116">Application</span></span>|<span data-ttu-id="e13e9-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e13e9-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e13e9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e13e9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e13e9-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e13e9-119">Optional query parameters</span></span>
<span data-ttu-id="e13e9-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e13e9-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e13e9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e13e9-121">Request headers</span></span>
|<span data-ttu-id="e13e9-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e13e9-122">Header</span></span>|<span data-ttu-id="e13e9-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e13e9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e13e9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e13e9-124">Authorization</span></span>|<span data-ttu-id="e13e9-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e13e9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e13e9-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e13e9-126">Accept</span></span>|<span data-ttu-id="e13e9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e13e9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e13e9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e13e9-128">Request body</span></span>
<span data-ttu-id="e13e9-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e13e9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e13e9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e13e9-130">Response</span></span>
<span data-ttu-id="e13e9-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e13e9-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e13e9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e13e9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e13e9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e13e9-133">Request</span></span>
<span data-ttu-id="e13e9-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e13e9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="e13e9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e13e9-135">Response</span></span>
<span data-ttu-id="e13e9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e13e9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "id": "a3883444-3444-a388-4434-88a3443488a3",
    "value": "Value value"
  }
}
```




