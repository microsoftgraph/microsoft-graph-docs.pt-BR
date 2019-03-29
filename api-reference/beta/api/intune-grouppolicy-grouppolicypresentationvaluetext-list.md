---
title: Listar groupPolicyPresentationValueTexts
description: Listar Propriedades e relações dos objetos groupPolicyPresentationValueText.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c857f1f6d7fc44f640649ea121b1be4c0a9753f6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965190"
---
# <a name="list-grouppolicypresentationvaluetexts"></a><span data-ttu-id="50f94-103">Listar groupPolicyPresentationValueTexts</span><span class="sxs-lookup"><span data-stu-id="50f94-103">List groupPolicyPresentationValueTexts</span></span>

> <span data-ttu-id="50f94-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50f94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50f94-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50f94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50f94-106">Listar Propriedades e relações dos objetos [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="50f94-106">List properties and relationships of the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50f94-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50f94-107">Prerequisites</span></span>
<span data-ttu-id="50f94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50f94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50f94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50f94-110">Permission type</span></span>|<span data-ttu-id="50f94-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50f94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50f94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50f94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50f94-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="50f94-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="50f94-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50f94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50f94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50f94-115">Not supported.</span></span>|
|<span data-ttu-id="50f94-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50f94-116">Application</span></span>|<span data-ttu-id="50f94-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50f94-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50f94-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50f94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="50f94-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50f94-119">Request headers</span></span>
|<span data-ttu-id="50f94-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50f94-120">Header</span></span>|<span data-ttu-id="50f94-121">Valor</span><span class="sxs-lookup"><span data-stu-id="50f94-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50f94-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="50f94-122">Authorization</span></span>|<span data-ttu-id="50f94-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50f94-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50f94-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50f94-124">Accept</span></span>|<span data-ttu-id="50f94-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50f94-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50f94-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50f94-126">Request body</span></span>
<span data-ttu-id="50f94-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50f94-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50f94-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="50f94-128">Response</span></span>
<span data-ttu-id="50f94-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50f94-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50f94-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50f94-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="50f94-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50f94-131">Request</span></span>
<span data-ttu-id="50f94-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50f94-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="50f94-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="50f94-133">Response</span></span>
<span data-ttu-id="50f94-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50f94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




