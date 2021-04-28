---
title: Gerenciar regras de monitoramento para uma implantação usando o serviço de implantação Windows Update for Business
description: Para implantações iniciadas pelo serviço de implantação, você pode usar regras de monitoramento que configurem alertas e ações automatizadas com base em sinais de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 7468bef695b704ef40b630e3f0e332e97fb12031
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067656"
---
# <a name="manage-monitoring-rules-for-a-feature-update-deployment-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="4173a-103">Gerenciar regras de monitoramento para uma implantação de atualização de recursos usando o serviço de implantação Windows Update for Business</span><span class="sxs-lookup"><span data-stu-id="4173a-103">Manage monitoring rules for a feature update deployment using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="4173a-104">Para implantações iniciadas pelo serviço de implantação, você pode usar uma regra de monitoramento para configurar alertas e ações automatizadas com base em sinais de implantação.</span><span class="sxs-lookup"><span data-stu-id="4173a-104">For deployments initiated by the deployment service, you can use a monitoring rule to configure alerts and automated actions based on deployment signals.</span></span>

<span data-ttu-id="4173a-105">As regras de monitoramento são compatíveis com implantações de Windows 10 de recursos.</span><span class="sxs-lookup"><span data-stu-id="4173a-105">Monitoring rules are compatible with deployments of Windows 10 feature updates.</span></span>

> [!NOTE]
> <span data-ttu-id="4173a-106">Se você não especificar uma regra [de monitoramento](/graph/api/resources/windowsupdates-monitoringrule) ao criar uma [implantação,](/graph/api/resources/windowsupdates-deployment)uma regra de monitoramento padrão será criada.</span><span class="sxs-lookup"><span data-stu-id="4173a-106">If you do not specify a [monitoring rule](/graph/api/resources/windowsupdates-monitoringrule) when creating a [deployment](/graph/api/resources/windowsupdates-deployment), a default monitoring rule is created.</span></span> <span data-ttu-id="4173a-107">Esta regra de monitoramento padrão tem **um sinal** de , `rollback` um **limite** de e `20` uma **ação** de `alertError` .</span><span class="sxs-lookup"><span data-stu-id="4173a-107">This default monitoring rule has a **signal** of `rollback`, a **threshold** of `20`, and an **action** of `alertError`.</span></span> <span data-ttu-id="4173a-108">Em uma atualização futura da API, esse comportamento mudará e uma regra de monitoramento padrão não será criada.</span><span class="sxs-lookup"><span data-stu-id="4173a-108">In a future update of the API, this behavior will change and a default monitoring rule will not be created.</span></span>

## <a name="step-1-create-a-monitoring-rule"></a><span data-ttu-id="4173a-109">Etapa 1: Criar uma regra de monitoramento</span><span class="sxs-lookup"><span data-stu-id="4173a-109">Step 1: Create a monitoring rule</span></span>

<span data-ttu-id="4173a-110">Você pode criar uma [regra de monitoramento para](/graph/api/resources/windowsupdates-monitoringrule) uma implantação configurando as [configurações de monitoramento.](/graph/api/resources/windowsupdates-monitoringsettings)</span><span class="sxs-lookup"><span data-stu-id="4173a-110">You can create a [monitoring rule](/graph/api/resources/windowsupdates-monitoringrule) for a deployment by configuring the [monitoring settings](/graph/api/resources/windowsupdates-monitoringsettings).</span></span> <span data-ttu-id="4173a-111">Cada [implantação](/graph/api/resources/windowsupdates-deployments) pode ter uma regra de monitoramento ativa por vez.</span><span class="sxs-lookup"><span data-stu-id="4173a-111">Each [deployment](/graph/api/resources/windowsupdates-deployments) can have one active monitoring rule at a time.</span></span>

<span data-ttu-id="4173a-112">As regras de monitoramento consistem em três componentes:</span><span class="sxs-lookup"><span data-stu-id="4173a-112">Monitoring rules consist of three components:</span></span>
* <span data-ttu-id="4173a-113">**sinal**: O tipo de problema de atualização a ser monitorado pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="4173a-113">**signal**: The type of update issue to be monitored by the deployment service.</span></span>
* <span data-ttu-id="4173a-114">**threshold**: Quando essa porcentagem de dispositivos emite o sinal especificado, a regra de monitoramento é disparada.</span><span class="sxs-lookup"><span data-stu-id="4173a-114">**threshold**: When this percentage of devices emit the specified signal, the monitoring rule is triggered.</span></span>
* <span data-ttu-id="4173a-115">**ação**: a ação a ser tomada quando a regra de monitoramento é disparada.</span><span class="sxs-lookup"><span data-stu-id="4173a-115">**action**: The action to take when the monitoring rule is triggered.</span></span>

<span data-ttu-id="4173a-116">Veja a seguir um exemplo de criação de uma regra de monitoramento para uma implantação ao mesmo tempo que a criação da implantação.</span><span class="sxs-lookup"><span data-stu-id="4173a-116">Below is an example of creating a monitoring rule for a deployment at the same time as creating the deployment.</span></span>

### <a name="request"></a><span data-ttu-id="4173a-117">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4173a-117">Request</span></span>

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
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

### <a name="response"></a><span data-ttu-id="4173a-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="4173a-118">Response</span></span>

```http
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
        "rollout": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-2-unpause-a-deployment-that-was-paused-by-a-monitoring-rule"></a><span data-ttu-id="4173a-119">Etapa 2: desempacotar uma implantação que foi pausada por uma regra de monitoramento</span><span class="sxs-lookup"><span data-stu-id="4173a-119">Step 2: Unpause a deployment that was paused by a monitoring rule</span></span>
<span data-ttu-id="4173a-120">Quando uma regra de monitoramento é acionada, ela oferece a oportunidade de investigar problemas de atualização que podem ter causado a aplicação.</span><span class="sxs-lookup"><span data-stu-id="4173a-120">When a monitoring rule triggers, it provides the opportunity to investigate update issues that may have lead to it being applied.</span></span> <span data-ttu-id="4173a-121">Após a investigação, talvez você queira retomar a implantação.</span><span class="sxs-lookup"><span data-stu-id="4173a-121">After investigation, you may wish to resume the deployment.</span></span> <span data-ttu-id="4173a-122">Há duas maneiras de fazer isso: remover a regra de monitoramento ou atualizar o limite da regra de monitoramento.</span><span class="sxs-lookup"><span data-stu-id="4173a-122">There are two ways to do so: removing the monitoring rule or updating the monitoring rule threshold.</span></span>

### <a name="example-resume-deployment-by-removing-a-monitoring-rule"></a><span data-ttu-id="4173a-123">Exemplo: retomar a implantação removendo uma regra de monitoramento</span><span class="sxs-lookup"><span data-stu-id="4173a-123">Example: Resume deployment by removing a monitoring rule</span></span>
<span data-ttu-id="4173a-124">Quando uma regra de monitoramento que pausa a implantação é disparada, uma maneira de retomar a implantação é remover a regra.</span><span class="sxs-lookup"><span data-stu-id="4173a-124">When a monitoring rule that pauses the deployment is triggered, one way to resume the deployment is to remove the rule.</span></span>

<span data-ttu-id="4173a-125">Veja a seguir um exemplo de retomada da implantação removendo a regra.</span><span class="sxs-lookup"><span data-stu-id="4173a-125">Below is an example of resuming the deployment by removing the rule.</span></span>

#### <a name="request"></a><span data-ttu-id="4173a-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4173a-126">Request</span></span>

``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": []
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="4173a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4173a-127">Response</span></span>

``` http
HTTP/1.1 202 Accepted
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
        "monitoring": {
            "monitoringRules": []
        },
        "rollout": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

### <a name="example-resume-deployment-by-updating-a-monitoring-rule-threshold"></a><span data-ttu-id="4173a-128">Exemplo: retomar a implantação atualizando um limite de regra de monitoramento</span><span class="sxs-lookup"><span data-stu-id="4173a-128">Example: Resume deployment by updating a monitoring rule threshold</span></span>
<span data-ttu-id="4173a-129">Outra maneira de retomar a implantação é alterar o limite da regra de monitoramento relevante.</span><span class="sxs-lookup"><span data-stu-id="4173a-129">Another way to resume the deployment is to change the threshold of the relevant monitoring rule.</span></span> <span data-ttu-id="4173a-130">Quando o novo limite for atingido, a ação (nesse `pauseDeployment` caso, ) será disparada novamente.</span><span class="sxs-lookup"><span data-stu-id="4173a-130">When the new threshold is reached, the action (in this case, `pauseDeployment`) will be triggered again.</span></span> 

<span data-ttu-id="4173a-131">Veja a seguir um exemplo de retomada da implantação alterando o limite da regra de monitoramento.</span><span class="sxs-lookup"><span data-stu-id="4173a-131">Below is an example of resuming the deployment by changing the monitoring rule threshold.</span></span> <span data-ttu-id="4173a-132">Este exemplo também ilustra como editar qualquer regra de monitoramento existente, mesmo que seu limite ainda não tenha sido atendido, bem como criar uma regra de monitoramento em uma implantação que não tenha uma.</span><span class="sxs-lookup"><span data-stu-id="4173a-132">This example also illustrates how to edit any existing monitoring rule, even if its threshold has not yet been met, as well as how to create a monitoring rule on a deployment that does not have one.</span></span>

#### <a name="request"></a><span data-ttu-id="4173a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4173a-133">Request</span></span>

``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
                    "signal": "rollback",
                    "threshold": 10,
                    "action": "pauseDeployment"
                }
            ]
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="4173a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4173a-134">Response</span></span>

``` http
HTTP/1.1 202 Accepted
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
        "monitoring": {
            "monitoringRules": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
                    "signal": "rollback",
                    "threshold": 10,
                    "action": "pauseDeployment"
                }
            ]
        },
        "rollout": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```