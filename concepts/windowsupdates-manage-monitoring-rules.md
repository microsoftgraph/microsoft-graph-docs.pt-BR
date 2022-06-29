---
title: Gerenciar regras de monitoramento usando o serviço Windows Update implantação do Windows Update Business
description: Use o Windows Update de implantação para Empresas para criar uma regra de monitoramento ou retomar implantações pausadas por uma regra de monitoramento.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 30f2c9cd2d219710fda5beba6862e9f15c7c94d6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437447"
---
# <a name="manage-monitoring-rules-using-the-windows-update-for-business-deployment-service"></a>Gerenciar regras de monitoramento usando o serviço Windows Update implantação do Windows Update Business

Para implantações iniciadas pelo serviço de implantação, você pode usar uma regra de monitoramento para configurar alertas e ações automatizadas com base em sinais de implantação.

As regras de monitoramento são compatíveis com implantações de Windows 10 de recursos.

## <a name="step-1-create-a-monitoring-rule"></a>Etapa 1: Criar uma regra de monitoramento

Você pode criar uma [regra de monitoramento para](/graph/api/resources/windowsupdates-monitoringrule) uma implantação definindo as [configurações de monitoramento](/graph/api/resources/windowsupdates-monitoringsettings). Cada [implantação](/graph/api/resources/windowsupdates-deployments) pode ter uma regra de monitoramento ativa por vez.

As regras de monitoramento consistem em três componentes:
* **sinal**: o tipo de problema de atualização a ser monitorado pelo serviço de implantação.
* **limite**: quando essa porcentagem de dispositivos emite o sinal especificado, a regra de monitoramento é disparada.
* **ação**: a ação a ser tomada quando a regra de monitoramento é disparada.

Veja abaixo um exemplo de como criar uma regra de monitoramento para uma implantação ao mesmo tempo que criar a implantação.

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
        "monitoring": {
            "monitoringRules": [
                {
                    "signal": "rollback",
                    "threshold": 5,
                    "action": "pauseDeployment"
                }
            ]
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
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-2-resume-a-deployment-that-was-paused-by-a-monitoring-rule"></a>Etapa 2: Retomar uma implantação que foi pausada por uma regra de monitoramento
Quando uma regra de monitoramento é disparada, ela fornece a oportunidade de investigar problemas de atualização que podem ter feito com que ela seja aplicada. Após a investigação, talvez você queira retomar a implantação. Há duas maneiras de fazer isso: remover a regra de monitoramento ou atualizar o limite da regra de monitoramento.

### <a name="example-resume-deployment-by-removing-a-monitoring-rule"></a>Exemplo: retomar a implantação removendo uma regra de monitoramento
Quando uma regra de monitoramento que pausa a implantação é disparada, uma maneira de retomar a implantação é remover a regra.

Veja abaixo um exemplo de retomada da implantação removendo a regra.

#### <a name="request"></a>Solicitação

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

#### <a name="response"></a>Resposta

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
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

### <a name="example-resume-deployment-by-updating-a-monitoring-rule-threshold"></a>Exemplo: retomar a implantação atualizando um limite de regra de monitoramento
Outra maneira de retomar a implantação é alterar o limite da regra de monitoramento relevante. Quando o novo limite for atingido, a ação (nesse caso, `pauseDeployment`) será disparada novamente. 

Veja abaixo um exemplo de retomada da implantação alterando o limite da regra de monitoramento. Este exemplo também ilustra como editar qualquer regra de monitoramento existente, mesmo que seu limite ainda não tenha sido atingido, bem como como criar uma regra de monitoramento em uma implantação que não tenha uma.

#### <a name="request"></a>Solicitação

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
                    "signal": "rollback",
                    "threshold": 10,
                    "action": "pauseDeployment"
                }
            ]
        }
    }
}
```

#### <a name="response"></a>Resposta

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
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```
