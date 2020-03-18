---
title: Listar groupPolicyUploadedDefinitions
description: Listar Propriedades e relações dos objetos groupPolicyUploadedDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01fd83bbd4aace0e6663fe4379341336af004400
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803740"
---
# <a name="list-grouppolicyuploadeddefinitions"></a><span data-ttu-id="df914-103">Listar groupPolicyUploadedDefinitions</span><span class="sxs-lookup"><span data-stu-id="df914-103">List groupPolicyUploadedDefinitions</span></span>

> <span data-ttu-id="df914-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df914-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df914-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df914-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df914-106">Listar Propriedades e relações dos objetos [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="df914-106">List properties and relationships of the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df914-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df914-107">Prerequisites</span></span>
<span data-ttu-id="df914-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df914-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df914-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df914-110">Permission type</span></span>|<span data-ttu-id="df914-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df914-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df914-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df914-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df914-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="df914-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="df914-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df914-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df914-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df914-115">Not supported.</span></span>|
|<span data-ttu-id="df914-116">Application</span><span class="sxs-lookup"><span data-stu-id="df914-116">Application</span></span>|<span data-ttu-id="df914-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="df914-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df914-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df914-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyDefinitions
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a><span data-ttu-id="df914-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df914-119">Request headers</span></span>
|<span data-ttu-id="df914-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df914-120">Header</span></span>|<span data-ttu-id="df914-121">Valor</span><span class="sxs-lookup"><span data-stu-id="df914-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df914-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df914-122">Authorization</span></span>|<span data-ttu-id="df914-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df914-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df914-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df914-124">Accept</span></span>|<span data-ttu-id="df914-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df914-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df914-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df914-126">Request body</span></span>
<span data-ttu-id="df914-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df914-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df914-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="df914-128">Response</span></span>
<span data-ttu-id="df914-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df914-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df914-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df914-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="df914-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df914-131">Request</span></span>
<span data-ttu-id="df914-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df914-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions
```

### <a name="response"></a><span data-ttu-id="df914-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="df914-133">Response</span></span>
<span data-ttu-id="df914-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df914-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
      "classType": "machine",
      "displayName": "Display Name value",
      "explainText": "Explain Text value",
      "categoryPath": "Category Path value",
      "supportedOn": "Supported On value",
      "policyType": "admxIngested",
      "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
      "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




