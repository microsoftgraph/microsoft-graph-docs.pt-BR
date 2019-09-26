---
title: Listar groupPolicyPresentationValueTexts
description: Listar Propriedades e relações dos objetos groupPolicyPresentationValueText.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 36ce7e5cd59a3e01840e72f549236d33805d69fa
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193434"
---
# <a name="list-grouppolicypresentationvaluetexts"></a><span data-ttu-id="046ce-103">Listar groupPolicyPresentationValueTexts</span><span class="sxs-lookup"><span data-stu-id="046ce-103">List groupPolicyPresentationValueTexts</span></span>

> <span data-ttu-id="046ce-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="046ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="046ce-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="046ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="046ce-106">Listar Propriedades e relações dos objetos [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="046ce-106">List properties and relationships of the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="046ce-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="046ce-107">Prerequisites</span></span>
<span data-ttu-id="046ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="046ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="046ce-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="046ce-110">Permission type</span></span>|<span data-ttu-id="046ce-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="046ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="046ce-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="046ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="046ce-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="046ce-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="046ce-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="046ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="046ce-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="046ce-115">Not supported.</span></span>|
|<span data-ttu-id="046ce-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="046ce-116">Application</span></span>|<span data-ttu-id="046ce-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="046ce-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="046ce-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="046ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="046ce-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="046ce-119">Request headers</span></span>
|<span data-ttu-id="046ce-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="046ce-120">Header</span></span>|<span data-ttu-id="046ce-121">Valor</span><span class="sxs-lookup"><span data-stu-id="046ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="046ce-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="046ce-122">Authorization</span></span>|<span data-ttu-id="046ce-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="046ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="046ce-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="046ce-124">Accept</span></span>|<span data-ttu-id="046ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="046ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="046ce-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="046ce-126">Request body</span></span>
<span data-ttu-id="046ce-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="046ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="046ce-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="046ce-128">Response</span></span>
<span data-ttu-id="046ce-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="046ce-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="046ce-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="046ce-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="046ce-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="046ce-131">Request</span></span>
<span data-ttu-id="046ce-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="046ce-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="046ce-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="046ce-133">Response</span></span>
<span data-ttu-id="046ce-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="046ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




