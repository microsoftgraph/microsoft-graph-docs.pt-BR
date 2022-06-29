---
title: Implantar uma atualização de recursos usando o serviço Windows Update implantação do Windows Update Business
description: Siga estas etapas para implantar atualizações de recursos do Windows em dispositivos em um locatário Azure AD usando o serviço de implantação do Windows Update for Business.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 176d4c07348b367bfe02335617ebae3328573907
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437503"
---
# <a name="deploy-a-feature-update-using-the-windows-update-for-business-deployment-service"></a>Implantar uma atualização de recursos usando o serviço Windows Update implantação do Windows Update Business

Com o serviço Windows Update implantação do Azure AD Business, você pode implantar atualizações do Windows em dispositivos em um Azure AD locatário. Atualmente, o serviço de implantação dá suporte a [implantações](windowsupdates-deployments.md) Windows 10 atualizações de recursos e atualizações de segurança aceleradas. Este tópico se concentra em implantações de atualizações de recursos. Para obter informações sobre como implantar atualizações de segurança aceleradas, consulte [Implantar uma atualização de segurança acelerada](windowsupdates-deploy-expedited-update.md).

Quando você implanta uma atualização de recurso em um dispositivo, Windows Update oferece a atualização especificada para o dispositivo se ele ainda não tiver recebido a atualização. Por exemplo, se você implantar uma atualização de recurso versão 20H2 do Windows 10 em um dispositivo registrado no gerenciamento de atualização de recursos e estiver atualmente em uma versão mais antiga do Windows 10, o dispositivo será atualizado para a versão 20H2. Se o dispositivo já estiver na versão 20H2 ou superior, ele permanecerá em sua versão atual. Se o dispositivo não estiver registrado no gerenciamento de atualização de recursos, o dispositivo não será afetado por essa operação.

Desde que um dispositivo permaneça registrado no gerenciamento de atualização de recursos, o dispositivo não receberá nenhuma outra atualização de recurso do Windows Update menos que seja implantado explicitamente usando o serviço de implantação.

> [!IMPORTANT]
> Ao usar o serviço de implantação do Windows Update for Business para atualizar dispositivos para o Windows 11 (definindo o parâmetro de versão de uma implantação como "Windows 11, versão 21H2"), você está concordando que, ao aplicar esse sistema operacional a um dispositivo (1), a licença do Windows aplicável foi adquirida por meio do licenciamento por volume ou (2) que você está autorizado a associar seu  e estão aceitando em seu nome os Termos de Licença de Software Microsoft relevantes para serem encontrados aqui: Termos [de Licença de Software da Microsoft](https://www.microsoft.com/Useterms).

## <a name="prerequisites"></a>Pré-requisitos

* Os dispositivos [atendem aos pré-requisitos para o serviço de implantação](windowsupdates-concept-overview.md#prerequisites).
* Antes de usar o serviço de implantação para implantar atualizações de recursos, os [](windowsupdates-enroll.md) dispositivos devem ser registrados no gerenciamento pelo serviço de implantação para a categoria de atualização de recursos.

## <a name="step-1-optional-get-a-list-of-deployable-updates"></a>Etapa 1: (Opcional) Obter uma lista de atualizações implantáveis

Você pode consultar o catálogo de serviços de implantação para obter uma lista de atualizações que podem ser implantadas em dispositivos como conteúdo em uma implantação.

Veja abaixo um exemplo de consulta para todas as Windows 10 de recursos que podem ser implantadas pelo serviço de implantação.

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

Uma [implantação](/graph/api/resources/windowsupdates-deployment) especifica o conteúdo a ser implantado, como e quando implantar o conteúdo e os dispositivos de destino. Quando uma implantação é criada, um público-alvo de implantação é criado automaticamente como uma relação.

Veja abaixo um exemplo de como criar uma implantação de uma atualização de recursos, com configurações opcionais definindo [o agendamento](windowsupdates-schedule-deployment.md) de implantação e [as regras de monitoramento](windowsupdates-manage-monitoring-rules.md). [As proteções](windowsupdates-manage-safeguards.md) são aplicadas por padrão. Os dispositivos de destino são especificados na próxima etapa.

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
        "safeguard": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-3-assign-devices-to-the-deployment-audience"></a>Etapa 3: Atribuir dispositivos ao público-alvo da implantação

Depois que uma implantação é criada, você pode atribuir dispositivos ao [público-alvo da implantação](/graph/api/resources/windowsupdates-deploymentaudience). Depois que o público-alvo da implantação for atualizado com êxito, o Windows Update começará a oferecer a atualização para os dispositivos relevantes de acordo com as configurações de implantação.

Os dispositivos são registrados automaticamente com o serviço quando adicionados às coleções de membros ou exclusões de um público-alvo de implantação (ou seja, um objeto [azureADDevice é criado automaticamente](/graph/api/resources/windowsupdates-azureaddevice) se ele ainda não existir).

O exemplo a seguir mostra como adicionar Azure AD como membros do público de implantação.

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

Enquanto uma implantação está em andamento, você pode pausar a implantação atualizando seu **estado, bem** como atualizar seus membros de audiência e exclusões.

## <a name="after-a-deployment"></a>Após uma implantação

Depois que todos os dispositivos atribuídos a um público de implantação tiverem sido inicialmente oferecidos à atualização, é possível que nem todos os dispositivos tenham iniciado ou concluído a atualização, devido a fatores como a conectividade do dispositivo. Desde que a implantação ainda exista, Windows Update continua a oferecer a atualização aos dispositivos atribuídos sempre que eles se reconectam.

