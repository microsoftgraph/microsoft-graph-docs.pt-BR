---
title: Listar groupPolicyPresentationTextBoxes
description: Listar Propriedades e relações dos objetos groupPolicyPresentationTextBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 946bca119dae89e6c89a7410728e70f3da42a176
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170123"
---
# <a name="list-grouppolicypresentationtextboxes"></a><span data-ttu-id="8f721-103">Listar groupPolicyPresentationTextBoxes</span><span class="sxs-lookup"><span data-stu-id="8f721-103">List groupPolicyPresentationTextBoxes</span></span>

> <span data-ttu-id="8f721-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8f721-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f721-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f721-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f721-106">Listar Propriedades e relações dos objetos [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="8f721-106">List properties and relationships of the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f721-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f721-107">Prerequisites</span></span>
<span data-ttu-id="8f721-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8f721-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8f721-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f721-110">Permission type</span></span>|<span data-ttu-id="8f721-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f721-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f721-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f721-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f721-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f721-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8f721-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f721-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f721-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f721-115">Not supported.</span></span>|
|<span data-ttu-id="8f721-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f721-116">Application</span></span>|<span data-ttu-id="8f721-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f721-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f721-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f721-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="8f721-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f721-119">Request headers</span></span>
|<span data-ttu-id="8f721-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f721-120">Header</span></span>|<span data-ttu-id="8f721-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8f721-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f721-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f721-122">Authorization</span></span>|<span data-ttu-id="8f721-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f721-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f721-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8f721-124">Accept</span></span>|<span data-ttu-id="8f721-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8f721-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f721-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f721-126">Request body</span></span>
<span data-ttu-id="8f721-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f721-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f721-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f721-128">Response</span></span>
<span data-ttu-id="8f721-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f721-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f721-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f721-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f721-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f721-131">Request</span></span>
<span data-ttu-id="8f721-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f721-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="8f721-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f721-133">Response</span></span>
<span data-ttu-id="8f721-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f721-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
      "label": "Label value",
      "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "defaultValue": "Default Value value",
      "required": true,
      "maxLength": 9
    }
  ]
}
```




