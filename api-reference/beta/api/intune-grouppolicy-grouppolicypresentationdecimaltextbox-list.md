---
title: Listar groupPolicyPresentationDecimalTextBoxes
description: Listar propriedades e relações dos objetos groupPolicyPresentationDecimalTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2141c03b02a38bec55497e6eb4362f1d9f6253f5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149636"
---
# <a name="list-grouppolicypresentationdecimaltextboxes"></a><span data-ttu-id="0fb20-103">Listar groupPolicyPresentationDecimalTextBoxes</span><span class="sxs-lookup"><span data-stu-id="0fb20-103">List groupPolicyPresentationDecimalTextBoxes</span></span>

<span data-ttu-id="0fb20-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fb20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fb20-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0fb20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fb20-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0fb20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fb20-107">Listar propriedades e relações dos [objetos groupPolicyPresentationDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)</span><span class="sxs-lookup"><span data-stu-id="0fb20-107">List properties and relationships of the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fb20-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0fb20-108">Prerequisites</span></span>
<span data-ttu-id="0fb20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fb20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fb20-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fb20-111">Permission type</span></span>|<span data-ttu-id="0fb20-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fb20-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fb20-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fb20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0fb20-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb20-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0fb20-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fb20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fb20-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fb20-116">Not supported.</span></span>|
|<span data-ttu-id="0fb20-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fb20-117">Application</span></span>|<span data-ttu-id="0fb20-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb20-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fb20-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fb20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="0fb20-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fb20-120">Request headers</span></span>
|<span data-ttu-id="0fb20-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fb20-121">Header</span></span>|<span data-ttu-id="0fb20-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0fb20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fb20-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fb20-123">Authorization</span></span>|<span data-ttu-id="0fb20-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fb20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fb20-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0fb20-125">Accept</span></span>|<span data-ttu-id="0fb20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0fb20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fb20-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fb20-127">Request body</span></span>
<span data-ttu-id="0fb20-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0fb20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fb20-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fb20-129">Response</span></span>
<span data-ttu-id="0fb20-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fb20-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fb20-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fb20-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fb20-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fb20-132">Request</span></span>
<span data-ttu-id="0fb20-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fb20-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="0fb20-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fb20-134">Response</span></span>
<span data-ttu-id="0fb20-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fb20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 407

{
  "value": [
    {
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
  ]
}
```




