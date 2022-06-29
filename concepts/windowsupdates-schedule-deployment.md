---
title: Agendar uma implantação usando o serviço Windows Update implantação do Windows Update Business
description: Ao implantar uma atualização, você pode agendar a implantação para que os dispositivos recebam a atualização posteriormente usando o serviço de implantação Windows Update for Business.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 60d505eb5fab2ef003bb04762b6cccf3974e4f25
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437384"
---
# <a name="schedule-a-deployment-using-the-windows-update-for-business-deployment-service"></a>Agendar uma implantação usando o serviço Windows Update implantação do Windows Update Business

Ao implantar uma atualização usando o serviço de implantação, você pode agendar a implantação para que os dispositivos recebam a atualização em uma data futura.

Os recursos de agendamento são [compatíveis com implantações](windowsupdates-deployments.md) de Windows 10 de recursos.

## <a name="schedule-a-deployment-to-start-at-a-future-date"></a>Agendar uma implantação para iniciar em uma data futura

Você pode agendar uma implantação para iniciar em uma data futura definindo suas [configurações de distribuição](/graph/api/resources/windowsupdates-rolloutsettings). No exemplo abaixo, todos os dispositivos atribuídos à implantação receberão a atualização em 1º de julho de 2021.

### <a name="request"></a>Solicitação

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

### <a name="response"></a>Resposta

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
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="stage-a-deployment-over-a-period-of-time"></a>Preparar uma implantação durante um período de tempo

Você também pode agendar uma implantação para que os dispositivos atribuídos sejam oferecidos à atualização em uma distribuição gradual que é preparada ao longo do tempo. A atualização é oferecida a subconjuntos de dispositivos atribuídos à implantação em intervalos regulares, com a duração total da distribuição determinada por uma data de término ou taxa de oferta. Você pode pensar em uma distribuição gradual como semelhante a uma série de eventos de calendário recorrente.

### <a name="example-stage-a-deployment-at-regular-intervals-between-start-and-end-dates"></a>Exemplo: preparar uma implantação em intervalos regulares entre as datas de início e término

Uma maneira de preparar uma implantação ao longo do tempo é definir **o endDateTime** da implantação. Todos os dispositivos atribuídos à implantação receberão a atualização dentro da janela entre **startDateTime** e **endDateTime**. Se **startDateTime não** for especificado, a implantação começará assim que os dispositivos forem atribuídos.

Neste exemplo, você configura uma nova implantação para que um novo conjunto de dispositivos seja oferecido a atualização toda semana (**durationBetweenOffers** definido como sete dias), a partir de 1º de julho de 2021. Todos os dispositivos têm a atualização oferecida antes de 1º de agosto de 2021.

#### <a name="request"></a>Solicitação

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

#### <a name="response"></a>Resposta

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
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```


### <a name="example-stage-a-deployment-at-regular-intervals-with-a-specified-number-of-devices-at-each-offer"></a>Exemplo: preparar uma implantação em intervalos regulares com um número especificado de dispositivos em cada oferta

Outra maneira de preparar uma implantação ao longo do tempo é configurar a taxa de oferta usando `devicesPerOffer`. Os dispositivos atribuídos à implantação receberão a atualização de acordo com a taxa especificada até que todos os dispositivos tenham sido oferecidos a atualização.

Neste exemplo, você configura uma nova implantação para que um novo conjunto de dispositivos seja oferecido a atualização toda semana (**durationBetweenOffers** definido como sete dias), a partir de 1º de julho de 2021. 100 dispositivos são oferecidos a atualização por vez até que todos os dispositivos tenham sido oferecidos a atualização.

#### <a name="request"></a>Solicitação

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

#### <a name="response"></a>Resposta

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
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```
