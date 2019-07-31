---
title: Obter groupPolicyPresentationLongDecimalTextBox
description: Leia as propriedades e as relações do objeto groupPolicyPresentationLongDecimalTextBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09c960aa085d7e1a21607008f7da5703728df16d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989424"
---
# <a name="get-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="55009-103">Obter groupPolicyPresentationLongDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="55009-103">Get groupPolicyPresentationLongDecimalTextBox</span></span>

> <span data-ttu-id="55009-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55009-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55009-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55009-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55009-106">Leia as propriedades e as relações do objeto [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="55009-106">Read properties and relationships of the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55009-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55009-107">Prerequisites</span></span>
<span data-ttu-id="55009-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55009-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55009-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55009-110">Permission type</span></span>|<span data-ttu-id="55009-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55009-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55009-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55009-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55009-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="55009-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="55009-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55009-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55009-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55009-115">Not supported.</span></span>|
|<span data-ttu-id="55009-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55009-116">Application</span></span>|<span data-ttu-id="55009-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55009-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55009-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55009-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55009-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55009-119">Optional query parameters</span></span>
<span data-ttu-id="55009-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="55009-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55009-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55009-121">Request headers</span></span>
|<span data-ttu-id="55009-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55009-122">Header</span></span>|<span data-ttu-id="55009-123">Valor</span><span class="sxs-lookup"><span data-stu-id="55009-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55009-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="55009-124">Authorization</span></span>|<span data-ttu-id="55009-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55009-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55009-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55009-126">Accept</span></span>|<span data-ttu-id="55009-127">application/json</span><span class="sxs-lookup"><span data-stu-id="55009-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55009-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55009-128">Request body</span></span>
<span data-ttu-id="55009-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55009-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55009-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="55009-130">Response</span></span>
<span data-ttu-id="55009-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55009-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55009-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55009-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="55009-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55009-133">Request</span></span>
<span data-ttu-id="55009-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55009-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="55009-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="55009-135">Response</span></span>
<span data-ttu-id="55009-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55009-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 377

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
    "label": "Label value",
    "id": "754d8495-8495-754d-9584-4d7595844d75",
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





