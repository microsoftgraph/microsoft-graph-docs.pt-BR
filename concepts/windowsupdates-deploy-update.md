---
title: Implantar uma atualização de recurso usando o serviço de implantação Windows Atualização para Empresas
description: Com o Windows de implantação do Update for Business, você pode implantar Windows de recursos em dispositivos em um locatário do Azure AD.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 872b0e0a4b8acc0d31821be7a21283c7dc2e70ca
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61859900"
---
# <a name="deploy-a-feature-update-using-the-windows-update-for-business-deployment-service"></a>Implantar uma atualização de recurso usando o serviço de implantação Windows Atualização para Empresas

Com o Windows de implantação do Update for Business, você pode implantar Windows atualizações em dispositivos em um locatário do Azure AD. Hoje, o serviço de implantação oferece suporte a [implantações](windowsupdates-deployments.md) de Windows 10 de recursos e atualizações de segurança rápidas. Este tópico se concentra em implantações de atualizações de recursos. Para obter informações sobre como implantar atualizações de segurança aceleradas, consulte [Deploy an expedited security update](windowsupdates-deploy-expedited-update.md).

Quando você implanta uma atualização de recurso em um dispositivo, o Windows Update oferece a atualização especificada para o dispositivo se ainda não tiver recebido a atualização. Por exemplo, se você implantar Windows 10 versão 20H2 de atualização de recursos em um dispositivo que está inscrito no gerenciamento de atualização de recursos e está atualmente em uma versão mais antiga do Windows 10, o dispositivo será atualizado para a versão 20H2. Se o dispositivo já estiver na versão 20H2 ou superior, ele permanecerá em sua versão atual. Se o dispositivo não estiver inscrito no gerenciamento de atualização de recursos, o dispositivo não será afetado por essa operação.

Enquanto um dispositivo permanecer inscrito no gerenciamento de atualização de recursos, o dispositivo não receberá outras atualizações de recursos do Windows Update, a menos que seja implantado explicitamente usando o serviço de implantação.

> [!IMPORTANT]
> Usando o serviço de implantação do Windows Update for Business para atualizar dispositivos para o Windows 11 (definindo o paramater de versão de uma implantação como "Windows 11, versão 21H2"), você concorda que ao aplicar esse sistema operacional a um dispositivo (1) o Windows  licença foi adquirida embora o licenciamento por volume, ou (2) que você está autorizado a vincular sua organização e está aceitando em seu nome os Termos de Licença de Software da Microsoft relevantes a serem encontrados aqui: Termos de Licença de Software da [Microsoft](https://www.microsoft.com/Useterms).

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

A seguir está um exemplo de criação de uma implantação de uma atualização de recursos, com configurações opcionais configurando o [cronograma](windowsupdates-schedule-deployment.md) de implantação e as regras [de monitoramento.](windowsupdates-manage-monitoring-rules.md) [As proteções](windowsupdates-manage-safeguards.md) são aplicadas por padrão. Os dispositivos direcionados são especificados na próxima etapa.

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

