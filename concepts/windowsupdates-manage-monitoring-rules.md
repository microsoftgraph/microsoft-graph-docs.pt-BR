---
title: Gerenciar regras de monitoramento para uma implantação usando o serviço de implantação Windows Update for Business
description: Para implantações iniciadas pelo serviço de implantação, você pode usar regras de monitoramento que configurem alertas e ações automatizadas com base em sinais de implantação.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 1e4f0538a9e7a5d47b070514685a11860a86ac35
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117526"
---
# <a name="manage-monitoring-rules-for-a-feature-update-deployment-using-the-windows-update-for-business-deployment-service"></a>Gerenciar regras de monitoramento para uma implantação de atualização de recursos usando o serviço de implantação Windows Update for Business

Para implantações iniciadas pelo serviço de implantação, você pode usar uma regra de monitoramento para configurar alertas e ações automatizadas com base em sinais de implantação.

As regras de monitoramento são compatíveis com implantações de Windows 10 de recursos.

> [!NOTE]
> Se você não especificar uma regra [de monitoramento](/graph/api/resources/windowsupdates-monitoringrule) ao criar uma [implantação,](/graph/api/resources/windowsupdates-deployment)uma regra de monitoramento padrão será criada. Esta regra de monitoramento padrão tem **um sinal** de , `rollback` um **limite** de e `20` uma **ação** de `alertError` . Em uma atualização futura da API, esse comportamento mudará e uma regra de monitoramento padrão não será criada.

## <a name="step-1-create-a-monitoring-rule"></a>Etapa 1: Criar uma regra de monitoramento

Você pode criar uma [regra de monitoramento para](/graph/api/resources/windowsupdates-monitoringrule) uma implantação configurando as [configurações de monitoramento.](/graph/api/resources/windowsupdates-monitoringsettings) Cada [implantação](/graph/api/resources/windowsupdates-deployments) pode ter uma regra de monitoramento ativa por vez.

As regras de monitoramento consistem em três componentes:
* **sinal**: O tipo de problema de atualização a ser monitorado pelo serviço de implantação.
* **threshold**: Quando essa porcentagem de dispositivos emite o sinal especificado, a regra de monitoramento é disparada.
* **ação**: a ação a ser tomada quando a regra de monitoramento é disparada.

Veja a seguir um exemplo de criação de uma regra de monitoramento para uma implantação ao mesmo tempo que a criação da implantação.

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-2-unpause-a-deployment-that-was-paused-by-a-monitoring-rule"></a>Etapa 2: desempacotar uma implantação que foi pausada por uma regra de monitoramento
Quando uma regra de monitoramento é acionada, ela oferece a oportunidade de investigar problemas de atualização que podem ter causado a aplicação. Após a investigação, talvez você queira retomar a implantação. Há duas maneiras de fazer isso: remover a regra de monitoramento ou atualizar o limite da regra de monitoramento.

### <a name="example-resume-deployment-by-removing-a-monitoring-rule"></a>Exemplo: retomar a implantação removendo uma regra de monitoramento
Quando uma regra de monitoramento que pausa a implantação é disparada, uma maneira de retomar a implantação é remover a regra.

Veja a seguir um exemplo de retomada da implantação removendo a regra.

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

### <a name="example-resume-deployment-by-updating-a-monitoring-rule-threshold"></a>Exemplo: retomar a implantação atualizando um limite de regra de monitoramento
Outra maneira de retomar a implantação é alterar o limite da regra de monitoramento relevante. Quando o novo limite for atingido, a ação (nesse `pauseDeployment` caso, ) será disparada novamente. 

Veja a seguir um exemplo de retomada da implantação alterando o limite da regra de monitoramento. Este exemplo também ilustra como editar qualquer regra de monitoramento existente, mesmo que seu limite ainda não tenha sido atendido, bem como criar uma regra de monitoramento em uma implantação que não tenha uma.

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```
