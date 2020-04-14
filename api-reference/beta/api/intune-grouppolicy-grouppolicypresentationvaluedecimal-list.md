---
title: Listar groupPolicyPresentationValueDecimals
description: Listar Propriedades e relações dos objetos groupPolicyPresentationValueDecimal.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 78cb2f23bc2dad12239ba3706cfd28b7fba1825c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460335"
---
# <a name="list-grouppolicypresentationvaluedecimals"></a><span data-ttu-id="837eb-103">Listar groupPolicyPresentationValueDecimals</span><span class="sxs-lookup"><span data-stu-id="837eb-103">List groupPolicyPresentationValueDecimals</span></span>

<span data-ttu-id="837eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="837eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="837eb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="837eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="837eb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="837eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="837eb-107">Listar Propriedades e relações dos objetos [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="837eb-107">List properties and relationships of the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="837eb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="837eb-108">Prerequisites</span></span>
<span data-ttu-id="837eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="837eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="837eb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="837eb-111">Permission type</span></span>|<span data-ttu-id="837eb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="837eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="837eb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="837eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="837eb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="837eb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="837eb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="837eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="837eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="837eb-116">Not supported.</span></span>|
|<span data-ttu-id="837eb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="837eb-117">Application</span></span>|<span data-ttu-id="837eb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="837eb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="837eb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="837eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="837eb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="837eb-120">Request headers</span></span>
|<span data-ttu-id="837eb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="837eb-121">Header</span></span>|<span data-ttu-id="837eb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="837eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="837eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="837eb-123">Authorization</span></span>|<span data-ttu-id="837eb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="837eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="837eb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="837eb-125">Accept</span></span>|<span data-ttu-id="837eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="837eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="837eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="837eb-127">Request body</span></span>
<span data-ttu-id="837eb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="837eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="837eb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="837eb-129">Response</span></span>
<span data-ttu-id="837eb-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="837eb-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="837eb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="837eb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="837eb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="837eb-132">Request</span></span>
<span data-ttu-id="837eb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="837eb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="837eb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="837eb-134">Response</span></span>
<span data-ttu-id="837eb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="837eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "id": "8821bede-bede-8821-debe-2188debe2188",
      "value": 5
    }
  ]
}
```



