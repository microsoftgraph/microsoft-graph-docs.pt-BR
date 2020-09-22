---
title: Listar groupPolicyPresentationValueTexts
description: Listar Propriedades e relações dos objetos groupPolicyPresentationValueText.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1c38049ae80b70143ea7499f5988f76229ecfc62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082452"
---
# <a name="list-grouppolicypresentationvaluetexts"></a><span data-ttu-id="f4b2f-103">Listar groupPolicyPresentationValueTexts</span><span class="sxs-lookup"><span data-stu-id="f4b2f-103">List groupPolicyPresentationValueTexts</span></span>

<span data-ttu-id="f4b2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4b2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4b2f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4b2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4b2f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4b2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4b2f-107">Listar Propriedades e relações dos objetos [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f4b2f-107">List properties and relationships of the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4b2f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4b2f-108">Prerequisites</span></span>
<span data-ttu-id="f4b2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4b2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4b2f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4b2f-111">Permission type</span></span>|<span data-ttu-id="f4b2f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4b2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4b2f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4b2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4b2f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4b2f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f4b2f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4b2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4b2f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4b2f-116">Not supported.</span></span>|
|<span data-ttu-id="f4b2f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4b2f-117">Application</span></span>|<span data-ttu-id="f4b2f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4b2f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4b2f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4b2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="f4b2f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4b2f-120">Request headers</span></span>
|<span data-ttu-id="f4b2f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4b2f-121">Header</span></span>|<span data-ttu-id="f4b2f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f4b2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4b2f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4b2f-123">Authorization</span></span>|<span data-ttu-id="f4b2f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4b2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4b2f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4b2f-125">Accept</span></span>|<span data-ttu-id="f4b2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4b2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4b2f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4b2f-127">Request body</span></span>
<span data-ttu-id="f4b2f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f4b2f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4b2f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4b2f-129">Response</span></span>
<span data-ttu-id="f4b2f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4b2f-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4b2f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4b2f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4b2f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4b2f-132">Request</span></span>
<span data-ttu-id="f4b2f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4b2f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="f4b2f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4b2f-134">Response</span></span>
<span data-ttu-id="f4b2f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4b2f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 326

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "id": "a3883444-3444-a388-4434-88a3443488a3",
      "value": "Value value"
    }
  ]
}
```






