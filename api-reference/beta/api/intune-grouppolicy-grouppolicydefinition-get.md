---
title: Obter groupPolicyDefinition
description: Leia propriedades e relações do objeto groupPolicyDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: edacf2e3c699e4562b1ce830d566081bfa51ce79
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145779"
---
# <a name="get-grouppolicydefinition"></a><span data-ttu-id="dc271-103">Obter groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="dc271-103">Get groupPolicyDefinition</span></span>

<span data-ttu-id="dc271-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc271-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc271-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc271-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc271-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc271-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc271-107">Leia propriedades e relações do [objeto groupPolicyDefinition.](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dc271-107">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc271-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc271-108">Prerequisites</span></span>
<span data-ttu-id="dc271-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc271-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc271-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc271-111">Permission type</span></span>|<span data-ttu-id="dc271-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc271-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc271-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc271-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc271-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc271-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc271-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc271-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc271-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc271-116">Not supported.</span></span>|
|<span data-ttu-id="dc271-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc271-117">Application</span></span>|<span data-ttu-id="dc271-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc271-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc271-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc271-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions/{groupPolicyDefinitionId}
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc271-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dc271-120">Optional query parameters</span></span>
<span data-ttu-id="dc271-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dc271-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc271-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc271-122">Request headers</span></span>
|<span data-ttu-id="dc271-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc271-123">Header</span></span>|<span data-ttu-id="dc271-124">Valor</span><span class="sxs-lookup"><span data-stu-id="dc271-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc271-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc271-125">Authorization</span></span>|<span data-ttu-id="dc271-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc271-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc271-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc271-127">Accept</span></span>|<span data-ttu-id="dc271-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dc271-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc271-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc271-129">Request body</span></span>
<span data-ttu-id="dc271-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc271-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc271-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc271-131">Response</span></span>
<span data-ttu-id="dc271-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc271-132">If successful, this method returns a `200 OK` response code and [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc271-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc271-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc271-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc271-134">Request</span></span>
<span data-ttu-id="dc271-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc271-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
```

### <a name="response"></a><span data-ttu-id="dc271-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc271-136">Response</span></span>
<span data-ttu-id="dc271-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc271-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 505

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyDefinition",
    "classType": "machine",
    "displayName": "Display Name value",
    "explainText": "Explain Text value",
    "categoryPath": "Category Path value",
    "supportedOn": "Supported On value",
    "policyType": "admxIngested",
    "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
    "id": "f9607947-7947-f960-4779-60f9477960f9",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




