---
title: Criar implantação
description: Crie um novo objeto de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 5c2b9c4a228aa33b7bf5ff134a43b265a8e01486
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067252"
---
# <a name="create-deployment"></a><span data-ttu-id="c6eec-103">Criar implantação</span><span class="sxs-lookup"><span data-stu-id="c6eec-103">Create deployment</span></span>
<span data-ttu-id="c6eec-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c6eec-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!NOTE]
> <span data-ttu-id="c6eec-105">Se você não especificar uma regra [de monitoramento](/graph/api/resources/windowsupdates-monitoringrule) ao criar uma implantação, uma regra de monitoramento padrão será criada.</span><span class="sxs-lookup"><span data-stu-id="c6eec-105">If you do not specify a [monitoring rule](/graph/api/resources/windowsupdates-monitoringrule) when creating a deployment, a default monitoring rule is created.</span></span> <span data-ttu-id="c6eec-106">Esta regra de monitoramento padrão tem **um sinal** de , `rollback` um **limite** de e `20` uma **ação** de `alertError` .</span><span class="sxs-lookup"><span data-stu-id="c6eec-106">This default monitoring rule has a **signal** of `rollback`, a **threshold** of `20`, and an **action** of `alertError`.</span></span> <span data-ttu-id="c6eec-107">Em uma atualização futura da API, esse comportamento mudará e uma regra de monitoramento padrão não será criada.</span><span class="sxs-lookup"><span data-stu-id="c6eec-107">In a future update of the API, this behavior will change and a default monitoring rule will not be created.</span></span>

<span data-ttu-id="c6eec-108">Crie um novo [objeto de implantação.](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="c6eec-108">Create a new [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6eec-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6eec-109">Permissions</span></span>
<span data-ttu-id="c6eec-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6eec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6eec-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6eec-112">Permission type</span></span>|<span data-ttu-id="c6eec-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6eec-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6eec-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6eec-114">Delegated (work or school account)</span></span>|<span data-ttu-id="c6eec-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6eec-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="c6eec-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6eec-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6eec-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6eec-117">Not supported.</span></span>|
|<span data-ttu-id="c6eec-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6eec-118">Application</span></span>|<span data-ttu-id="c6eec-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6eec-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6eec-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6eec-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments
```

## <a name="request-headers"></a><span data-ttu-id="c6eec-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6eec-121">Request headers</span></span>
|<span data-ttu-id="c6eec-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c6eec-122">Name</span></span>|<span data-ttu-id="c6eec-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6eec-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c6eec-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6eec-124">Authorization</span></span>|<span data-ttu-id="c6eec-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6eec-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c6eec-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6eec-127">Content-Type</span></span>|<span data-ttu-id="c6eec-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6eec-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6eec-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6eec-130">Request body</span></span>
<span data-ttu-id="c6eec-131">No corpo da solicitação, fornece uma representação JSON do [objeto de](../resources/windowsupdates-deployment.md) implantação.</span><span class="sxs-lookup"><span data-stu-id="c6eec-131">In the request body, supply a JSON representation of the [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

<span data-ttu-id="c6eec-132">A tabela a seguir mostra as propriedades necessárias ao criar a [implantação](../resources/windowsupdates-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="c6eec-132">The following table shows the properties that are required when you create the [deployment](../resources/windowsupdates-deployment.md).</span></span>

|<span data-ttu-id="c6eec-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6eec-133">Property</span></span>|<span data-ttu-id="c6eec-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6eec-134">Type</span></span>|<span data-ttu-id="c6eec-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6eec-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6eec-136">content</span><span class="sxs-lookup"><span data-stu-id="c6eec-136">content</span></span>|[<span data-ttu-id="c6eec-137">microsoft.graph.windowsUpdates.deployableContent</span><span class="sxs-lookup"><span data-stu-id="c6eec-137">microsoft.graph.windowsUpdates.deployableContent</span></span>](../resources/windowsupdates-deployablecontent.md)|<span data-ttu-id="c6eec-138">Especifica qual conteúdo implantar.</span><span class="sxs-lookup"><span data-stu-id="c6eec-138">Specifies what content to deploy.</span></span> <span data-ttu-id="c6eec-139">O conteúdo implantável deve ser fornecido como um dos seguintes tipos derivados: [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md) , [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md)</span><span class="sxs-lookup"><span data-stu-id="c6eec-139">Deployable content should be provided as one of the following derived types: [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md) , [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c6eec-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6eec-140">Response</span></span>

<span data-ttu-id="c6eec-141">Se tiver êxito, este método retornará um código de resposta e um `201 Created` objeto [de](../resources/windowsupdates-deployment.md) implantação no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6eec-141">If successful, this method returns a `201 Created` response code and a [deployment](../resources/windowsupdates-deployment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c6eec-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c6eec-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c6eec-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6eec-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_deployment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-Type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "rollout": {
      "devicesPerOffer": 100
    },
    "monitoring": {
      "monitoringRules": [
        {
          "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
          "signal": "rollback",
          "threshold": 5,
          "action": "pauseDeployment"
        }
      ]
    }
  }
}
```


### <a name="response"></a><span data-ttu-id="c6eec-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6eec-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "b5171742-1742-b517-4217-17b5421717b5",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
    "value": "offering",
    "reasons": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
        "value": "offeringByRequest"
      }
    ],
    "requestedValue": "none",
    "effectiveSinceDate": "String (timestamp)"
    },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "rollout": {
      "devicesPerOffer": 100,
      "durationBetweenOffers": "P7D",
      "startDateTime": null,
      "endDateTime": null
    },
    "monitoring": {
      "monitoringRules": [
        {
          "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
          "signal": "rollback",
          "threshold": 5,
          "action": "pauseDeployment"
        }
      ]
    },
    "userExperience": null
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

