---
title: Obter groupPolicyPresentationDecimalTextBox
description: Leia as propriedades e as relações do objeto groupPolicyPresentationDecimalTextBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3051fdbe440d9f98032ca561ed85aa47bb90f541
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087009"
---
# <a name="get-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="33735-103">Obter groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="33735-103">Get groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="33735-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33735-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33735-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33735-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33735-106">Leia as propriedades e as relações do objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="33735-106">Read properties and relationships of the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33735-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33735-107">Prerequisites</span></span>
<span data-ttu-id="33735-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33735-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33735-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33735-110">Permission type</span></span>|<span data-ttu-id="33735-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33735-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33735-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33735-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33735-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="33735-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="33735-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33735-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33735-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33735-115">Not supported.</span></span>|
|<span data-ttu-id="33735-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33735-116">Application</span></span>|<span data-ttu-id="33735-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="33735-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33735-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33735-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33735-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="33735-119">Optional query parameters</span></span>
<span data-ttu-id="33735-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="33735-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33735-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33735-121">Request headers</span></span>
|<span data-ttu-id="33735-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33735-122">Header</span></span>|<span data-ttu-id="33735-123">Valor</span><span class="sxs-lookup"><span data-stu-id="33735-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33735-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="33735-124">Authorization</span></span>|<span data-ttu-id="33735-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33735-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33735-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33735-126">Accept</span></span>|<span data-ttu-id="33735-127">application/json</span><span class="sxs-lookup"><span data-stu-id="33735-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33735-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33735-128">Request body</span></span>
<span data-ttu-id="33735-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33735-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33735-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="33735-130">Response</span></span>
<span data-ttu-id="33735-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33735-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33735-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33735-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="33735-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33735-133">Request</span></span>
<span data-ttu-id="33735-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33735-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="33735-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="33735-135">Response</span></span>
<span data-ttu-id="33735-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33735-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 373

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
    "label": "Label value",
    "id": "988daea7-aea7-988d-a7ae-8d98a7ae8d98",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "defaultValue": 12,
    "spin": true,
    "spinStep": 8,
    "required": true,
    "minValue": 8,
    "maxValue": 8
  }
}
```






