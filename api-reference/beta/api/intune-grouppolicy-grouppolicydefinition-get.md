---
title: Obter groupPolicyDefinition
description: Leia as propriedades e as relações do objeto groupPolicyDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 811baa15f7abcfa9857827f621b13be01464578c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306006"
---
# <a name="get-grouppolicydefinition"></a><span data-ttu-id="16a22-103">Obter groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="16a22-103">Get groupPolicyDefinition</span></span>

<span data-ttu-id="16a22-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16a22-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16a22-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="16a22-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16a22-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16a22-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16a22-107">Leia as propriedades e as relações do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="16a22-107">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16a22-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16a22-108">Prerequisites</span></span>
<span data-ttu-id="16a22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16a22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16a22-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16a22-111">Permission type</span></span>|<span data-ttu-id="16a22-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16a22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16a22-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16a22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16a22-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="16a22-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="16a22-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16a22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16a22-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16a22-116">Not supported.</span></span>|
|<span data-ttu-id="16a22-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16a22-117">Application</span></span>|<span data-ttu-id="16a22-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="16a22-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16a22-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16a22-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="16a22-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="16a22-120">Optional query parameters</span></span>
<span data-ttu-id="16a22-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="16a22-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16a22-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16a22-122">Request headers</span></span>
|<span data-ttu-id="16a22-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16a22-123">Header</span></span>|<span data-ttu-id="16a22-124">Valor</span><span class="sxs-lookup"><span data-stu-id="16a22-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16a22-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="16a22-125">Authorization</span></span>|<span data-ttu-id="16a22-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16a22-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16a22-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16a22-127">Accept</span></span>|<span data-ttu-id="16a22-128">application/json</span><span class="sxs-lookup"><span data-stu-id="16a22-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16a22-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16a22-129">Request body</span></span>
<span data-ttu-id="16a22-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16a22-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16a22-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="16a22-131">Response</span></span>
<span data-ttu-id="16a22-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16a22-132">If successful, this method returns a `200 OK` response code and [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16a22-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16a22-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="16a22-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16a22-134">Request</span></span>
<span data-ttu-id="16a22-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16a22-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
```

### <a name="response"></a><span data-ttu-id="16a22-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="16a22-136">Response</span></span>
<span data-ttu-id="16a22-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16a22-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




