---
title: Implantar uma atualização de recurso usando o serviço de implantação Windows Atualização para Empresas
description: Com o Windows de implantação do Update for Business, você pode implantar Windows de recursos em dispositivos em um locatário do Azure AD.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 59e3c5351ed88cebe76ee9c66fa99563379065af36b2b96e67c44600b279f6ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54225633"
---
# <a name="deploy-a-feature-update-using-the-windows-update-for-business-deployment-service"></a>Implantar uma atualização de recurso usando o serviço de implantação Windows Atualização para Empresas

Com o Windows de implantação do Update for Business, você pode implantar Windows atualizações em dispositivos em um locatário do Azure AD. Hoje, o serviço de implantação oferece suporte a [implantações](windowsupdates-deployments.md) de Windows 10 de recursos e atualizações de segurança rápidas. Este tópico se concentra em implantações de atualizações de recursos. Para obter informações sobre como implantar atualizações de segurança aceleradas, consulte [Deploy an expedited security update](windowsupdates-deploy-expedited-update.md).

Quando você implanta uma atualização de recurso em um dispositivo, o Windows Update oferece a atualização especificada para o dispositivo se ainda não tiver recebido a atualização. Por exemplo, se você implantar Windows 10 versão 20H2 de atualização de recursos em um dispositivo que está inscrito no gerenciamento de atualização de recursos e está atualmente em uma versão mais antiga do Windows 10, o dispositivo será atualizado para a versão 20H2. Se o dispositivo já estiver na versão 20H2 ou superior, ele permanecerá em sua versão atual. Se o dispositivo não estiver inscrito no gerenciamento de atualização de recursos, o dispositivo não será afetado por essa operação.

Enquanto um dispositivo permanecer inscrito no gerenciamento de atualização de recursos, o dispositivo não receberá outras atualizações de recursos do Windows Update, a menos que seja implantado explicitamente usando o serviço de implantação.

## <a name="prerequisites"></a>Pré-requisitos

* Os dispositivos [atendem aos pré-requisitos do serviço de implantação](windowsupdates-concept-overview.md#prerequisites).
* Antes de usar o serviço de implantação para [](windowsupdates-enroll.md) implantar atualizações de recursos, os dispositivos devem estar inscritos no gerenciamento pelo serviço de implantação para a categoria de atualização de recursos.

## <a name="step-1-optional-get-a-list-of-deployable-updates"></a>Etapa 1: (Opcional) Obter uma lista de atualizações implantáveis

Você pode consultar o catálogo de serviços de implantação para obter uma lista de atualizações que podem ser implantadas em dispositivos como conteúdo em uma implantação.

Veja a seguir um exemplo de consulta para todas as Windows 10 de recursos que podem ser implantadas pelo serviço de implantação.

### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$filter=isof('microsoft.graph.windowsUpdates.featureUpdateCatalogEntry')
```

### <a name="response"></a>Resposta

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
            "id": "560a186a-1434-4364-8330-deb944b494ff",
            "displayName": "Windows 10, version 20H2",
            "releaseDate": "String (timestamp)",
            "deployableUntilDateTime": "String (timestamp)",
            "version": "20H2"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
            "id": "5e436dae-56bd-4925-bf8b-acf550e07227",
            "displayName": "Windows 10, version 2004",
            "releaseDate": "String (timestamp)",
            "deployableUntilDateTime": "String (timestamp)",
            "version": "2004"
        }
    ]
}
```

## <a name="step-2-create-a-deployment"></a>Etapa 2: Criar uma implantação

Uma [implantação](/graph/api/resources/windowsupdates-deployment) especifica o conteúdo a ser implantado, como e quando implantar o conteúdo e os dispositivos direcionados. Quando uma implantação é criada, uma audiência de implantação é criada automaticamente como uma relação.

A seguir está um exemplo de criação de uma implantação de uma atualização de recursos, com configurações opcionais configurando o [cronograma](windowsupdates-schedule-deployment.md) de implantação e as regras [de monitoramento.](windowsupdates-manage-monitoring-rules.md) Os dispositivos direcionados são especificados na próxima etapa.

> [!NOTE]
> Se você não especificar uma regra [de monitoramento](/graph/api/resources/windowsupdates-monitoringrule) ao criar uma implantação, uma regra de monitoramento padrão será criada. Esta regra de monitoramento padrão tem **um sinal** de , `rollback` um **limite** de e `20` uma **ação** de `alertError` . Em uma atualização futura da API, esse comportamento mudará e uma regra de monitoramento padrão não será criada.

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
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D"
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

## <a name="step-3-assign-devices-to-the-deployment-audience"></a>Etapa 3: Atribuir dispositivos à audiência de implantação

Após a criação de uma implantação, você pode atribuir dispositivos à audiência [de implantação.](/graph/api/resources/windowsupdates-deploymentaudience) Depois que o público de implantação é atualizado com êxito, o Windows Update começa a oferecer a atualização para os dispositivos relevantes de acordo com as configurações de implantação.

Os dispositivos são registrados automaticamente com o serviço quando adicionados aos membros ou coleções de exclusões de um público de implantação (ou seja, um [objeto azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) é criado automaticamente se ainda não existir).

O exemplo a seguir mostra como adicionar dispositivos do Azure AD como membros da audiência de implantação.

### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
Content-type: application/json

{
    "addMembers": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
            "id": "String (identifier)"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
            "id": "String (identifier)"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
            "id": "String (identifier)"
        }
    ]
}
```

### <a name="response"></a>Resposta

```http
HTTP/1.1 202 Accepted
```

## <a name="during-a-deployment"></a>Durante uma implantação

Enquanto uma implantação está em andamento, você pode pausar a implantação atualizando seu estado **,** bem como atualizar seus membros de audiência e exclusões.

## <a name="after-a-deployment"></a>Após uma implantação

Depois que todos os dispositivos atribuídos a um público de implantação foram inicialmente oferecidos a atualização, é possível que nem todos os dispositivos tenham iniciado ou concluído a atualização, devido a fatores como a conectividade do dispositivo. Enquanto a implantação ainda existir, o Windows Update continuará a oferecer a atualização para os dispositivos atribuídos sempre que eles se reconectam.

