---
title: Listar groupPolicyPresentationDecimalTextBoxes
description: Listar Propriedades e relações dos objetos groupPolicyPresentationDecimalTextBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b716f60ee0e072dc23d59935725b0b0d8a6a8076
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32531233"
---
# <a name="list-grouppolicypresentationdecimaltextboxes"></a><span data-ttu-id="d0eb3-103">Listar groupPolicyPresentationDecimalTextBoxes</span><span class="sxs-lookup"><span data-stu-id="d0eb3-103">List groupPolicyPresentationDecimalTextBoxes</span></span>

> <span data-ttu-id="d0eb3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d0eb3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0eb3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0eb3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0eb3-106">Listar Propriedades e relações dos objetos [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="d0eb3-106">List properties and relationships of the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0eb3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0eb3-107">Prerequisites</span></span>
<span data-ttu-id="d0eb3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0eb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0eb3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0eb3-110">Permission type</span></span>|<span data-ttu-id="d0eb3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d0eb3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0eb3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0eb3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0eb3-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0eb3-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d0eb3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0eb3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0eb3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0eb3-115">Not supported.</span></span>|
|<span data-ttu-id="d0eb3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0eb3-116">Application</span></span>|<span data-ttu-id="d0eb3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0eb3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0eb3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0eb3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="d0eb3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0eb3-119">Request headers</span></span>
|<span data-ttu-id="d0eb3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0eb3-120">Header</span></span>|<span data-ttu-id="d0eb3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d0eb3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0eb3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0eb3-122">Authorization</span></span>|<span data-ttu-id="d0eb3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0eb3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0eb3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0eb3-124">Accept</span></span>|<span data-ttu-id="d0eb3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0eb3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0eb3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0eb3-126">Request body</span></span>
<span data-ttu-id="d0eb3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0eb3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0eb3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0eb3-128">Response</span></span>
<span data-ttu-id="d0eb3-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0eb3-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0eb3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0eb3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0eb3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0eb3-131">Request</span></span>
<span data-ttu-id="d0eb3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0eb3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="d0eb3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0eb3-133">Response</span></span>
<span data-ttu-id="d0eb3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0eb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





