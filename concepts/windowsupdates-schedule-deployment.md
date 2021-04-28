---
title: Agendar uma implantação usando o serviço de implantação Windows Atualização para Empresas
description: Ao implantar uma atualização usando o serviço de implantação, você pode agendar a implantação para que os dispositivos recebam a atualização em uma data futura.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 461b40ef1e25d6a1943c70456404e7a48bf73d8c
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067655"
---
# <a name="schedule-a-deployment-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="1112d-103">Agendar uma implantação usando o serviço de implantação Windows Atualização para Empresas</span><span class="sxs-lookup"><span data-stu-id="1112d-103">Schedule a deployment using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="1112d-104">Ao implantar uma atualização usando o serviço de implantação, você pode agendar a implantação para que os dispositivos recebam a atualização em uma data futura.</span><span class="sxs-lookup"><span data-stu-id="1112d-104">When deploying an update using the deployment service, you can schedule the deployment so that devices receive the update at a future date.</span></span>

<span data-ttu-id="1112d-105">Os recursos de agendamento são compatíveis [com implantações](windowsupdates-deployments.md) de Windows 10 de recursos.</span><span class="sxs-lookup"><span data-stu-id="1112d-105">Scheduling features are compatible with [deployments](windowsupdates-deployments.md) of Windows 10 feature updates.</span></span>

## <a name="schedule-a-deployment-to-start-at-a-future-date"></a><span data-ttu-id="1112d-106">Agendar uma implantação para iniciar em uma data futura</span><span class="sxs-lookup"><span data-stu-id="1112d-106">Schedule a deployment to start at a future date</span></span>

<span data-ttu-id="1112d-107">Você pode agendar uma implantação para iniciar em uma data futura configurando suas configurações [de distribuição.](/graph/api/resources/windowsupdates-rolloutsettings)</span><span class="sxs-lookup"><span data-stu-id="1112d-107">You can schedule a deployment to start at a future date by configuring its [rollout settings](/graph/api/resources/windowsupdates-rolloutsettings).</span></span> <span data-ttu-id="1112d-108">No exemplo abaixo, todos os dispositivos atribuídos à implantação receberão a atualização em 1º de julho de 2021.</span><span class="sxs-lookup"><span data-stu-id="1112d-108">In the example below, all devices assigned the deployment will be offered the update on July 1, 2021.</span></span>

### <a name="request"></a><span data-ttu-id="1112d-109">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1112d-109">Request</span></span>

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
        "rollout": {
            "startDateTime": "2021-07-01T17:00:00Z",
        }
    }
}
```

### <a name="response"></a><span data-ttu-id="1112d-110">Resposta</span><span class="sxs-lookup"><span data-stu-id="1112d-110">Response</span></span>

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
        "rollout": {
            "startDateTime": "2021-07-01T17:00:00Z",
            "endDateTime": null,
            "durationBetweenOffers": "P1D",
            "devicesPerOffer": null
        },
        "monitoring": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="stage-a-deployment-over-a-period-of-time"></a><span data-ttu-id="1112d-111">Estágio de uma implantação por um período de tempo</span><span class="sxs-lookup"><span data-stu-id="1112d-111">Stage a deployment over a period of time</span></span>

<span data-ttu-id="1112d-112">Você também pode agendar uma implantação para que os dispositivos atribuídos sejam oferecidos a atualização em uma distribuição gradual que é em estágios ao longo do tempo.</span><span class="sxs-lookup"><span data-stu-id="1112d-112">You can also schedule a deployment so that assigned devices are offered the update in a gradual rollout that is staged over time.</span></span> <span data-ttu-id="1112d-113">A atualização é oferecida aos subconjunto de dispositivos atribuídos à implantação em intervalos regulares, com a duração total da distribuição determinada por uma data de término ou taxa de oferta.</span><span class="sxs-lookup"><span data-stu-id="1112d-113">The update is offered to subsets of devices assigned to the deployment at regular intervals, with the total duration of the rollout determined by either an end date or offering rate.</span></span> <span data-ttu-id="1112d-114">Você pode pensar em uma rollout gradual como semelhante a uma série de eventos de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="1112d-114">You can think of a gradual rollout as similar to a recurring calendar event series.</span></span>

### <a name="example-stage-a-deployment-at-regular-intervals-between-start-and-end-dates"></a><span data-ttu-id="1112d-115">Exemplo: estágio uma implantação em intervalos regulares entre as datas inicial e final</span><span class="sxs-lookup"><span data-stu-id="1112d-115">Example: Stage a deployment at regular intervals between start and end dates</span></span>

<span data-ttu-id="1112d-116">Uma maneira de estágio de uma implantação ao longo do tempo é definir **o endDateTime** da implantação.</span><span class="sxs-lookup"><span data-stu-id="1112d-116">One way to stage a deployment over time is to set the **endDateTime** of the deployment.</span></span> <span data-ttu-id="1112d-117">Todos os dispositivos atribuídos à implantação serão oferecidos a atualização dentro da janela entre **startDateTime** e **endDateTime**.</span><span class="sxs-lookup"><span data-stu-id="1112d-117">All devices assigned to the deployment will be offered the update within the window between the **startDateTime** and **endDateTime**.</span></span> <span data-ttu-id="1112d-118">Se o **startDateTime** não for especificado, a implantação começará assim que os dispositivos são atribuídos.</span><span class="sxs-lookup"><span data-stu-id="1112d-118">If the **startDateTime** is not specified, then the deployment will begin as soon as devices are assigned.</span></span>


<span data-ttu-id="1112d-119">Neste exemplo, você configura uma nova implantação para que um novo conjunto de dispositivos seja oferecido a atualização toda semana (**durationBetweenOffers** definida como sete dias), começando em 1º de julho de 2021.</span><span class="sxs-lookup"><span data-stu-id="1112d-119">In this example, you configure a new deployment so that a new set of devices is offered the update every week (**durationBetweenOffers** set to seven days), starting on July 1, 2021.</span></span> <span data-ttu-id="1112d-120">Todos os dispositivos são oferecidos a atualização antes de 1º de agosto de 2021.</span><span class="sxs-lookup"><span data-stu-id="1112d-120">All devices are offered the update before August 1, 2021.</span></span>

#### <a name="request"></a><span data-ttu-id="1112d-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1112d-121">Request</span></span>

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
        "rollout": {
            "startDateTime": "2021-07-01T17:00:00Z",
            "endDateTime": "2021-08-01T17:00:00Z",
            "durationBetweenOffers": "P7D"
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="1112d-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="1112d-122">Response</span></span>

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
        "rollout": {
            "startDateTime": "2021-07-01T17:00:00Z",
            "endDateTime": "2021-08-01T17:00:00Z",
            "durationBetweenOffers": "P7D",
            "devicesPerOffer": null
        },
        "monitoring": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```


### <a name="example-stage-a-deployment-at-regular-intervals-with-a-specified-number-of-devices-at-each-offer"></a><span data-ttu-id="1112d-123">Exemplo: estágio uma implantação em intervalos regulares com um número especificado de dispositivos em cada oferta</span><span class="sxs-lookup"><span data-stu-id="1112d-123">Example: Stage a deployment at regular intervals with a specified number of devices at each offer</span></span>

<span data-ttu-id="1112d-124">Outra maneira de estágio de uma implantação ao longo do tempo é configurar a taxa de oferta usando `devicesPerOffer` .</span><span class="sxs-lookup"><span data-stu-id="1112d-124">Another way to stage a deployment over time is to configure the offering rate using `devicesPerOffer`.</span></span> <span data-ttu-id="1112d-125">Os dispositivos atribuídos à implantação receberão a atualização de acordo com a taxa especificada até que todos os dispositivos tenham sido oferecidos a atualização.</span><span class="sxs-lookup"><span data-stu-id="1112d-125">Devices assigned to the deployment will be offered the update according to the specified rate until all devices have been offered the update.</span></span>

<span data-ttu-id="1112d-126">Neste exemplo, você configura uma nova implantação para que um novo conjunto de dispositivos seja oferecido a atualização toda semana (**durationBetweenOffers** definida como sete dias), começando em 1º de julho de 2021.</span><span class="sxs-lookup"><span data-stu-id="1112d-126">In this example, you configure a new deployment so that a new set of devices is offered the update every week (**durationBetweenOffers** set to seven days), starting on July 1, 2021.</span></span> <span data-ttu-id="1112d-127">100 dispositivos são oferecidos a atualização por vez até que todos os dispositivos tenham sido oferecidos a atualização.</span><span class="sxs-lookup"><span data-stu-id="1112d-127">100 devices are offered the update at a time until all devices have been offered the update.</span></span>

#### <a name="request"></a><span data-ttu-id="1112d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1112d-128">Request</span></span>

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
        "rollout": {
            "startDateTime": "2020-07-01T17:00:00Z",
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D"
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="1112d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1112d-129">Response</span></span>

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
        "rollout": {
            "startDateTime": "2020-07-01T17:00:00Z",
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D",
            "endDateTime": null
        },
        "monitoring": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```