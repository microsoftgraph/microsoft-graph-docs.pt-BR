---
title: Obter groupPolicyPresentationValueDecimal
description: Leia as propriedades e as relações do objeto groupPolicyPresentationValueDecimal.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 31a645a600624f07b18985cb23d3fb3d59ec9b90
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086946"
---
# <a name="get-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="2ad04-103">Obter groupPolicyPresentationValueDecimal</span><span class="sxs-lookup"><span data-stu-id="2ad04-103">Get groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="2ad04-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ad04-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ad04-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ad04-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ad04-106">Leia as propriedades e as relações do objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="2ad04-106">Read properties and relationships of the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ad04-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ad04-107">Prerequisites</span></span>
<span data-ttu-id="2ad04-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ad04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ad04-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ad04-110">Permission type</span></span>|<span data-ttu-id="2ad04-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ad04-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ad04-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ad04-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ad04-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ad04-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2ad04-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ad04-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ad04-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ad04-115">Not supported.</span></span>|
|<span data-ttu-id="2ad04-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ad04-116">Application</span></span>|<span data-ttu-id="2ad04-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ad04-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ad04-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ad04-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ad04-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ad04-119">Optional query parameters</span></span>
<span data-ttu-id="2ad04-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2ad04-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ad04-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ad04-121">Request headers</span></span>
|<span data-ttu-id="2ad04-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ad04-122">Header</span></span>|<span data-ttu-id="2ad04-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2ad04-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ad04-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ad04-124">Authorization</span></span>|<span data-ttu-id="2ad04-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ad04-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ad04-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ad04-126">Accept</span></span>|<span data-ttu-id="2ad04-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2ad04-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ad04-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ad04-128">Request body</span></span>
<span data-ttu-id="2ad04-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ad04-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ad04-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ad04-130">Response</span></span>
<span data-ttu-id="2ad04-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ad04-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ad04-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ad04-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ad04-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ad04-133">Request</span></span>
<span data-ttu-id="2ad04-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ad04-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="2ad04-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ad04-135">Response</span></span>
<span data-ttu-id="2ad04-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ad04-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "id": "8821bede-bede-8821-debe-2188debe2188",
    "value": 5
  }
}
```






