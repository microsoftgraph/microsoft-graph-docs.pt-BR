---
title: Listar groupPolicyPresentationMultiTextBoxes
description: Listar Propriedades e relações dos objetos groupPolicyPresentationMultiTextBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7fa7b2d3425327f5607dd2fe9db47d3eb0ef1ae
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977237"
---
# <a name="list-grouppolicypresentationmultitextboxes"></a><span data-ttu-id="07ede-103">Listar groupPolicyPresentationMultiTextBoxes</span><span class="sxs-lookup"><span data-stu-id="07ede-103">List groupPolicyPresentationMultiTextBoxes</span></span>

> <span data-ttu-id="07ede-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07ede-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07ede-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07ede-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07ede-106">Listar Propriedades e relações dos objetos [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="07ede-106">List properties and relationships of the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07ede-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07ede-107">Prerequisites</span></span>
<span data-ttu-id="07ede-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07ede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07ede-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07ede-110">Permission type</span></span>|<span data-ttu-id="07ede-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07ede-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07ede-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07ede-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07ede-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="07ede-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="07ede-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07ede-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07ede-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07ede-115">Not supported.</span></span>|
|<span data-ttu-id="07ede-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07ede-116">Application</span></span>|<span data-ttu-id="07ede-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07ede-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07ede-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07ede-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="07ede-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07ede-119">Request headers</span></span>
|<span data-ttu-id="07ede-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07ede-120">Header</span></span>|<span data-ttu-id="07ede-121">Valor</span><span class="sxs-lookup"><span data-stu-id="07ede-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07ede-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="07ede-122">Authorization</span></span>|<span data-ttu-id="07ede-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07ede-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07ede-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07ede-124">Accept</span></span>|<span data-ttu-id="07ede-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07ede-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07ede-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07ede-126">Request body</span></span>
<span data-ttu-id="07ede-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07ede-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07ede-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="07ede-128">Response</span></span>
<span data-ttu-id="07ede-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07ede-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07ede-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07ede-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="07ede-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07ede-131">Request</span></span>
<span data-ttu-id="07ede-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07ede-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="07ede-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="07ede-133">Response</span></span>
<span data-ttu-id="07ede-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07ede-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
      "label": "Label value",
      "id": "381ac035-c035-381a-35c0-1a3835c01a38",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "required": true,
      "maxLength": 9,
      "maxStrings": 10
    }
  ]
}
```




