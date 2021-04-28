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
# <a name="schedule-a-deployment-using-the-windows-update-for-business-deployment-service"></a>Agendar uma implantação usando o serviço de implantação Windows Atualização para Empresas

Ao implantar uma atualização usando o serviço de implantação, você pode agendar a implantação para que os dispositivos recebam a atualização em uma data futura.

Os recursos de agendamento são compatíveis [com implantações](windowsupdates-deployments.md) de Windows 10 de recursos.

## <a name="schedule-a-deployment-to-start-at-a-future-date"></a>Agendar uma implantação para iniciar em uma data futura

Você pode agendar uma implantação para iniciar em uma data futura configurando suas configurações [de distribuição.](/graph/api/resources/windowsupdates-rolloutsettings) No exemplo abaixo, todos os dispositivos atribuídos à implantação receberão a atualização em 1º de julho de 2021.

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="stage-a-deployment-over-a-period-of-time"></a>Estágio de uma implantação por um período de tempo

Você também pode agendar uma implantação para que os dispositivos atribuídos sejam oferecidos a atualização em uma distribuição gradual que é em estágios ao longo do tempo. A atualização é oferecida aos subconjunto de dispositivos atribuídos à implantação em intervalos regulares, com a duração total da distribuição determinada por uma data de término ou taxa de oferta. Você pode pensar em uma rollout gradual como semelhante a uma série de eventos de calendário recorrente.

### <a name="example-stage-a-deployment-at-regular-intervals-between-start-and-end-dates"></a>Exemplo: estágio uma implantação em intervalos regulares entre as datas inicial e final

Uma maneira de estágio de uma implantação ao longo do tempo é definir **o endDateTime** da implantação. Todos os dispositivos atribuídos à implantação serão oferecidos a atualização dentro da janela entre **startDateTime** e **endDateTime**. Se o **startDateTime** não for especificado, a implantação começará assim que os dispositivos são atribuídos.


Neste exemplo, você configura uma nova implantação para que um novo conjunto de dispositivos seja oferecido a atualização toda semana (**durationBetweenOffers** definida como sete dias), começando em 1º de julho de 2021. Todos os dispositivos são oferecidos a atualização antes de 1º de agosto de 2021.

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```


### <a name="example-stage-a-deployment-at-regular-intervals-with-a-specified-number-of-devices-at-each-offer"></a>Exemplo: estágio uma implantação em intervalos regulares com um número especificado de dispositivos em cada oferta

Outra maneira de estágio de uma implantação ao longo do tempo é configurar a taxa de oferta usando `devicesPerOffer` . Os dispositivos atribuídos à implantação receberão a atualização de acordo com a taxa especificada até que todos os dispositivos tenham sido oferecidos a atualização.

Neste exemplo, você configura uma nova implantação para que um novo conjunto de dispositivos seja oferecido a atualização toda semana (**durationBetweenOffers** definida como sete dias), começando em 1º de julho de 2021. 100 dispositivos são oferecidos a atualização por vez até que todos os dispositivos tenham sido oferecidos a atualização.

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```