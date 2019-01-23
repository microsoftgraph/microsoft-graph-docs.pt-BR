---
title: Lista groupPolicyPresentationLongDecimalTextBoxes
description: Lista as propriedades e os relacionamentos dos objetos groupPolicyPresentationLongDecimalTextBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 184225f7f0474da47f619aef0a52443e81469a67
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429253"
---
# <a name="list-grouppolicypresentationlongdecimaltextboxes"></a><span data-ttu-id="2d3ff-103">Lista groupPolicyPresentationLongDecimalTextBoxes</span><span class="sxs-lookup"><span data-stu-id="2d3ff-103">List groupPolicyPresentationLongDecimalTextBoxes</span></span>

> <span data-ttu-id="2d3ff-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2d3ff-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2d3ff-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2d3ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d3ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2d3ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d3ff-107">Lista as propriedades e os relacionamentos dos objetos [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="2d3ff-107">List properties and relationships of the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d3ff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d3ff-108">Prerequisites</span></span>
<span data-ttu-id="2d3ff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2d3ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2d3ff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d3ff-111">Permission type</span></span>|<span data-ttu-id="2d3ff-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d3ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d3ff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d3ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d3ff-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d3ff-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2d3ff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d3ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d3ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d3ff-116">Not supported.</span></span>|
|<span data-ttu-id="2d3ff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d3ff-117">Application</span></span>|<span data-ttu-id="2d3ff-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d3ff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d3ff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d3ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="2d3ff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d3ff-120">Request headers</span></span>
|<span data-ttu-id="2d3ff-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d3ff-121">Header</span></span>|<span data-ttu-id="2d3ff-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2d3ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d3ff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d3ff-123">Authorization</span></span>|<span data-ttu-id="2d3ff-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d3ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d3ff-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d3ff-125">Accept</span></span>|<span data-ttu-id="2d3ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d3ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d3ff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d3ff-127">Request body</span></span>
<span data-ttu-id="2d3ff-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2d3ff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d3ff-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d3ff-129">Response</span></span>
<span data-ttu-id="2d3ff-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d3ff-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d3ff-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d3ff-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d3ff-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d3ff-132">Request</span></span>
<span data-ttu-id="2d3ff-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d3ff-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="2d3ff-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d3ff-134">Response</span></span>
<span data-ttu-id="2d3ff-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d3ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 411

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
      "label": "Label value",
      "id": "754d8495-8495-754d-9584-4d7595844d75",
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




