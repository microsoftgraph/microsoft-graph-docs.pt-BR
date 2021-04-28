---
title: Implantar uma atualização de segurança acelerada usando o serviço de implantação Windows Update for Business
description: Com o serviço de implantação do Windows Update for Business, você pode implantar atualizações de segurança Windows em dispositivos em um locatário do Azure AD caso surja uma emergência e você precise implantar imediatamente uma atualização de segurança.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 9b8f3d341f94c0c2309e9c2674cfee41ddc34a9b
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067647"
---
# <a name="deploy-an-expedited-security-update-using-the-windows-update-for-business-deployment-service"></a>Implantar uma atualização de segurança acelerada usando o serviço de implantação Windows Update for Business

Com o Windows de implantação do Update for Business, você pode implantar Windows atualizações em dispositivos em um locatário do Azure AD. Hoje, o serviço de implantação oferece suporte a [implantações](windowsupdates-deployments.md) de Windows 10 de recursos e atualizações de segurança rápidas. Este tópico se concentra em implantações de atualizações de segurança aceleradas. Para obter informações sobre como implantar atualizações de recursos, consulte [Deploy a feature update](windowsupdates-deploy-update.md).

Agilizar uma atualização de segurança substitui Windows políticas de adiamento do Update for Business para que a atualização seja instalada o mais rápido possível. Ele pode ser útil quando surgirem eventos críticos de segurança e você precisar implantar as atualizações mais recentes mais rapidamente do que o normal. No entanto, embora possa ajudar a atingir metas de conformidade em relação a uma atualização de segurança específica, ela não foi projetada para ser usada todos os meses. Em vez disso, considere o [uso de prazos de conformidade para atualizações.](https://docs.microsoft.com/windows/deployment/update/wufb-compliancedeadlines)

Quando você implanta uma atualização de segurança acelerada em um dispositivo, o Windows Update oferece a atualização aplicável mais recente ao dispositivo se ainda não tiver recebido a atualização com a data de lançamento especificada. Por exemplo, se você implantar a atualização de segurança Windows 10 lançada em 13 de abril de 2021 em um dispositivo que não tenha a atualização no momento, o dispositivo receberá uma atualização acelerada. Se o dispositivo já tiver a atualização especificada ou mais recente, ele não receberá uma atualização acelerada.

Atualizações de segurança aceleradas também têm as seguintes características:

* A atualização começa imediatamente, em vez de aguardar a próxima verificação de atualização regular, que ocorre uma vez a cada 22 horas por padrão.
* A atualização baixa e instala o mais rápido possível.
* O processo de atualização substitui configurações de política de dispositivo, como dias até que o dispositivo seja forçado a reiniciar. Depois que a atualização acelerada é instalada, o dispositivo retorna às configurações de política atuais.

## <a name="prerequisites"></a>Pré-requisitos

* Os dispositivos [atendem aos pré-requisitos do serviço de implantação](windowsupdates-concept-overview.md#prerequisites).
* Os dispositivos instalaram a atualização descrita em [KB4023057 Windows 10 -](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a) Atualização para componentes do Serviço de Atualização (ou mais recente).

## <a name="step-1-optional-get-a-list-of-expeditable-updates"></a>Etapa 1: (Opcional) Obter uma lista de atualizações de conveniência

Você pode consultar o catálogo de serviços de implantação para obter uma lista de atualizações que podem ser aceleradas para dispositivos como conteúdo em uma implantação.

As atualizações de segurança são representadas pelo [tipo qualityUpdateCatalogEntry,](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) com **uma qualityUpdateClassification** de `security` . Todas Windows 10 de qualidade classificadas como atualizações de segurança podem ser aceleradas e marcadas com a **propriedade isExpeditable** definida para `true` identificá-las.

Veja a seguir um exemplo de consulta para todas as Windows 10 de segurança que podem ser implantadas como atualizações aceleradas pelo serviço de implantação. A Microsoft recomenda mostrar apenas as três atualizações mais atuais, portanto, o exemplo inclui `$top=3` .

### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$top=3&$filter=isof('microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry') and microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry/isExpeditable eq true&$orderby=releaseDateTime desc
```

### <a name="response"></a>Resposta

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
            "id": "bd9554dc-2737-4e3c-b794-fa2b8b3f4a30",
            "displayName": "MM/DD/YYYY - YYYY.MM B Security Updates for Windows 10",
            "releaseDateTime": "String (timestamp)",
            "deployableUntilDateTime": null,
            "isExpeditable": true,
            "qualityUpdateClassification": "security"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
            "id": "68860630-c2d0-4dd2-8c4b-9b9737ee5081",
            "displayName": "MM/DD/YYYY - YYYY.MM B Security Updates for Windows 10",
            "releaseDateTime": "String (timestamp)",
            "deployableUntilDateTime": null,
            "isExpeditable": true,
            "qualityUpdateClassification": "security"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
            "id": "aa336b13-db33-4d94-89ea-90e43e4ad30b",
            "displayName": "MM/DD/YYYY - YYYY.MM B Security Updates for Windows 10",
            "releaseDateTime": "String (timestamp)",
            "deployableUntilDateTime": null,
            "isExpeditable": true,
            "qualityUpdateClassification": "security"
        }
    ]
}
```

## <a name="step-2-create-a-deployment"></a>Etapa 2: Criar uma implantação

> [!NOTE]
> Na primeira vez que você implantar uma atualização de segurança acelerada em seu locatário, poderá ter até um atraso de um dia enquanto o serviço estiver configurado para sua organização. Esse atraso não se aplica a implantações ou implantações subsequentes de atualizações de recursos e será abordado em uma atualização futura.

Uma [implantação](/graph/api/resources/windowsupdates-deployment) especifica o conteúdo a ser implantado, como e quando implantar o conteúdo e os dispositivos direcionados. Para atualizações de qualidade, o conteúdo é especificado usando uma data de conformidade de destino. Quando uma implantação é criada, uma audiência de implantação é criada automaticamente como uma relação.

Quando você implanta uma atualização de segurança acelerada em um dispositivo, o Windows Update oferece uma atualização que traz o dispositivo acima do nível mínimo de conformidade especificado. Dependendo de quando cada dispositivo verifica e atualiza, alguns dispositivos podem receber atualizações mais novas (por exemplo, se houver uma atualização de segurança mais recente do que a correspondente ao nível mínimo de conformidade desejado), mas todos os dispositivos atendem ao padrão de conformidade de atualização de segurança especificado. Esse comportamento de oferecer a atualização aplicável mais recente, indicada pela propriedade **equivalentContent** que está sendo definida como o valor padrão, ajuda a manter os dispositivos o mais seguros possível e impede que um dispositivo receba uma atualização acelerada seguida por outra atualização regular apenas dias `latestSecurity` depois.

Você pode configurar o período de carência de reinicialização do dispositivo usando os dias da **propriedadeUntilForcedReboot** nas configurações de experiência [do](/graph/api/resources/windowsupdates-userexperiencesettings) usuário da implantação. O período de carência define a quantidade de tempo após a instalação que o usuário pode controlar o tempo de quando o dispositivo é reiniciado. Se o dispositivo não tiver reiniciado quando o período de carência expirar, ele será reiniciado automaticamente.

A seguir está um exemplo de criação de uma implantação para uma atualização de qualidade acelerada. Os dispositivos direcionados são especificados na próxima etapa.

### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
        "releaseDate": "YYYY-MM-DD"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "userExperience": {
            "daysUntilForcedReboot": 2
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
        "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
        "releaseDate": "YYYY-MM-DDT00:00:00Z",
        "classification": "security",
        "equivalentContent": "latestSecurity"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "userExperience": {
            "daysUntilForcedReboot": 2
        },
        "monitoring": null,
        "rollout": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-3-assign-devices-to-the-deployment-audience"></a>Etapa 3: Atribuir dispositivos à audiência de implantação

Após a criação de uma implantação, você pode atribuir dispositivos à audiência [de implantação.](/graph/api/resources/windowsupdates-deploymentaudience) Os dispositivos podem ser atribuídos diretamente ou por meio de [grupos de ativos atualizáveis.](/graph/api/resources/windowsupdates-updatableassetgroup) Depois que a audiência de implantação é atualizada com êxito, o Windows Update começa a oferecer a atualização para os dispositivos relevantes de acordo com as configurações de implantação.

Os dispositivos são registrados automaticamente com o serviço quando adicionados aos membros ou coleções de exclusões de um público de implantação (ou seja, um [objeto azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) é criado automaticamente se ainda não existir).

Veja a seguir um exemplo de adição de grupos de ativos atualizáveis e dispositivos do Azure AD como membros da audiência de implantação, além de excluir um dispositivo específico do Azure AD.

### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
Content-type: application/json

{
    "addMembers": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
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
    ],
    "addExclusions": [
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

Depois que todos os dispositivos atribuídos a um público de implantação foram inicialmente oferecidos a atualização, é possível que nem todos os dispositivos tenham iniciado ou concluído a atualização, devido a fatores como a conectividade do dispositivo. Enquanto a implantação ainda existir, ela continuará a garantir que o Windows Update esteja oferecendo a atualização para os dispositivos atribuídos sempre que eles se reconectam.
