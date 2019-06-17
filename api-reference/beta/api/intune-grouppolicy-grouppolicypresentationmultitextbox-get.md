---
title: Obter groupPolicyPresentationMultiTextBox
description: Leia as propriedades e as relações do objeto groupPolicyPresentationMultiTextBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6871bff0c583c3668dc572e26b9daa07ff6def65
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964560"
---
# <a name="get-grouppolicypresentationmultitextbox"></a><span data-ttu-id="f1556-103">Obter groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="f1556-103">Get groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="f1556-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1556-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1556-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1556-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1556-106">Leia as propriedades e as relações do objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="f1556-106">Read properties and relationships of the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1556-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1556-107">Prerequisites</span></span>
<span data-ttu-id="f1556-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1556-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1556-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1556-110">Permission type</span></span>|<span data-ttu-id="f1556-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1556-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1556-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1556-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1556-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1556-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f1556-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1556-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1556-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1556-115">Not supported.</span></span>|
|<span data-ttu-id="f1556-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1556-116">Application</span></span>|<span data-ttu-id="f1556-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1556-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1556-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1556-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1556-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1556-119">Optional query parameters</span></span>
<span data-ttu-id="f1556-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1556-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1556-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1556-121">Request headers</span></span>
|<span data-ttu-id="f1556-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1556-122">Header</span></span>|<span data-ttu-id="f1556-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f1556-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1556-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1556-124">Authorization</span></span>|<span data-ttu-id="f1556-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1556-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1556-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1556-126">Accept</span></span>|<span data-ttu-id="f1556-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f1556-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1556-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1556-128">Request body</span></span>
<span data-ttu-id="f1556-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1556-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1556-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1556-130">Response</span></span>
<span data-ttu-id="f1556-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1556-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1556-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1556-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1556-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1556-133">Request</span></span>
<span data-ttu-id="f1556-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1556-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="f1556-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1556-135">Response</span></span>
<span data-ttu-id="f1556-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1556-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 311

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
    "label": "Label value",
    "id": "381ac035-c035-381a-35c0-1a3835c01a38",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "required": true,
    "maxLength": 9,
    "maxStrings": 10
  }
}
```





