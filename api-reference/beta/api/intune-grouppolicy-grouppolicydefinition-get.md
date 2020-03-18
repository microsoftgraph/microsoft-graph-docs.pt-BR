---
title: Obter groupPolicyDefinition
description: Leia as propriedades e as relações do objeto groupPolicyDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 68ed972a88aa4d4b3dc2604bf79f6d5bc569da98
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804433"
---
# <a name="get-grouppolicydefinition"></a><span data-ttu-id="2bc8f-103">Obter groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="2bc8f-103">Get groupPolicyDefinition</span></span>

> <span data-ttu-id="2bc8f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2bc8f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bc8f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2bc8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bc8f-106">Leia as propriedades e as relações do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="2bc8f-106">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bc8f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2bc8f-107">Prerequisites</span></span>
<span data-ttu-id="2bc8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bc8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bc8f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bc8f-110">Permission type</span></span>|<span data-ttu-id="2bc8f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2bc8f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bc8f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bc8f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bc8f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bc8f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2bc8f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bc8f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bc8f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bc8f-115">Not supported.</span></span>|
|<span data-ttu-id="2bc8f-116">Application</span><span class="sxs-lookup"><span data-stu-id="2bc8f-116">Application</span></span>|<span data-ttu-id="2bc8f-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bc8f-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bc8f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bc8f-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="2bc8f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2bc8f-119">Optional query parameters</span></span>
<span data-ttu-id="2bc8f-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2bc8f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bc8f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bc8f-121">Request headers</span></span>
|<span data-ttu-id="2bc8f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2bc8f-122">Header</span></span>|<span data-ttu-id="2bc8f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2bc8f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bc8f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bc8f-124">Authorization</span></span>|<span data-ttu-id="2bc8f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bc8f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bc8f-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2bc8f-126">Accept</span></span>|<span data-ttu-id="2bc8f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2bc8f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bc8f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bc8f-128">Request body</span></span>
<span data-ttu-id="2bc8f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2bc8f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bc8f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bc8f-130">Response</span></span>
<span data-ttu-id="2bc8f-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bc8f-131">If successful, this method returns a `200 OK` response code and [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bc8f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bc8f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bc8f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bc8f-133">Request</span></span>
<span data-ttu-id="2bc8f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bc8f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
```

### <a name="response"></a><span data-ttu-id="2bc8f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bc8f-135">Response</span></span>
<span data-ttu-id="2bc8f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bc8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




