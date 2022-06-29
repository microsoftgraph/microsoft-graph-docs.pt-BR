---
title: Implantar uma atualização de segurança acelerada usando o serviço Windows Update implantação do Windows Update Business
description: Siga estas etapas para implantar atualizações de segurança do Windows aceleradas em dispositivos em um locatário Azure AD caso haja uma emergência usando o serviço de implantação do Windows Update for Business.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: c0c8d0389c2d152ebc4323639c0b8494927f89e7
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444212"
---
# <a name="deploy-an-expedited-security-update-using-the-windows-update-for-business-deployment-service"></a>Implantar uma atualização de segurança acelerada usando o serviço Windows Update implantação do Windows Update Business

Com o serviço Windows Update implantação do Azure AD Business, você pode implantar atualizações do Windows em dispositivos em um Azure AD locatário. Atualmente, o serviço de implantação dá suporte a [implantações](windowsupdates-deployments.md) Windows 10 atualizações de recursos e atualizações de segurança aceleradas. Este tópico se concentra em implantações de atualizações de segurança aceleradas. Para obter informações sobre como implantar atualizações de recursos, [consulte Implantar uma atualização de recursos](windowsupdates-deploy-update.md).

Agilizar uma atualização de segurança substitui Windows Update políticas de adiamento para Empresas para que a atualização seja instalada o mais rápido possível. Ele pode ser útil quando surgirem eventos de segurança críticos e você precisar implantar as atualizações mais recentes mais rapidamente do que o normal. No entanto, embora possa ajudar a atingir metas de conformidade em relação a uma atualização de segurança específica, ela não foi projetada para ser usada todos os meses. Em vez disso, considere [o uso de prazos de conformidade para atualizações](/windows/deployment/update/wufb-compliancedeadlines).

Quando você implanta uma atualização de segurança agilizada em um dispositivo, o Windows Update oferece a atualização aplicável mais recente ao dispositivo se ele ainda não tiver recebido a atualização com a data de lançamento especificada. Por exemplo, se você implantar a atualização de segurança do Windows 10 lançada em 13 de abril de 2021 em um dispositivo que não tenha a atualização no momento, o dispositivo receberá uma atualização acelerada. Se o dispositivo já tiver a atualização especificada ou mais recente, ele não receberá uma atualização acelerada.

As atualizações de segurança aceleradas também têm as seguintes características:

* A atualização é iniciada imediatamente em vez de aguardar a próxima verificação de atualização regular, que ocorre uma vez a cada 22 horas por padrão.
* A atualização é baixada e instalada o mais rápido possível.
* O processo de atualização substitui as configurações de política de dispositivo definidas, como dias até que o dispositivo seja forçado a reiniciar. Depois que a atualização acelerada é instalada, o dispositivo retorna para as configurações de política atuais.

## <a name="prerequisites"></a>Pré-requisitos

* Os dispositivos [atendem aos pré-requisitos para o serviço de implantação](windowsupdates-concept-overview.md#prerequisites).
* Os dispositivos instalaram a atualização descrita em [KB4023057 –](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a) Atualização para Windows 10 componentes do Serviço de Atualização (ou mais recente).

## <a name="step-1-optional-get-a-list-of-expeditable-updates"></a>Etapa 1: (Opcional) Obter uma lista de atualizações agilizáveis

Você pode consultar o catálogo de serviços de implantação para obter uma lista de atualizações que podem ser aceleradas para dispositivos como conteúdo em uma implantação.

As atualizações de segurança são representadas pelo tipo [qualityUpdateCatalogEntry](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) , com **uma qualityUpdateClassification** de `security`. Todas Windows 10 atualizações de qualidade classificadas como atualizações de segurança podem ser aceleradas e marcadas com a propriedade **isExpeditable** `true` definida para identificá-las.

Veja abaixo um exemplo de consulta para todas as Windows 10 de segurança que podem ser implantadas como atualizações aceleradas pelo serviço de implantação. A Microsoft recomenda mostrar apenas as três atualizações mais atuais, portanto, o exemplo inclui `$top=3`.

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

Uma [implantação](/graph/api/resources/windowsupdates-deployment) especifica o conteúdo a ser implantado, como e quando implantar o conteúdo e os dispositivos de destino. Para atualizações de qualidade, o conteúdo é especificado usando uma data de conformidade de destino. Quando uma implantação é criada, um público-alvo de implantação é criado automaticamente como uma relação.

Quando você implanta uma atualização de segurança acelerada em um dispositivo, o Windows Update oferece uma atualização que coloca o dispositivo acima do nível de conformidade mínimo especificado. Dependendo de quando cada dispositivo verifica e atualiza, alguns dispositivos podem receber atualizações mais recentes (por exemplo, se houver uma atualização de segurança mais recente do que a que corresponde ao nível de conformidade mínimo desejado), mas todos os dispositivos atendem ao padrão de conformidade de atualização de segurança especificado. Esse comportamento de oferecer a atualização aplicável mais recente, indicada pela propriedade **equivalentContent** `latestSecurity`que está sendo definida com o valor padrão, ajuda a manter os dispositivos o mais seguros possível e impede que um dispositivo receba uma atualização acelerada seguida por outra atualização regular apenas dias depois.

Você pode configurar o período de carência de reinicialização do dispositivo usando a propriedade **daysUntilForcedReboot** nas configurações de experiência [do](/graph/api/resources/windowsupdates-userexperiencesettings) usuário da implantação. O período de carência define a quantidade de tempo após a instalação que o usuário pode controlar o tempo de quando o dispositivo é reiniciado. Se o dispositivo não tiver reiniciado até o momento em que o período de carência expirar, ele será reiniciado automaticamente.

Veja abaixo um exemplo de como criar uma implantação para uma atualização de qualidade acelerada. Os dispositivos de destino são especificados na próxima etapa.

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
        "rollout": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-3-assign-devices-to-the-deployment-audience"></a>Etapa 3: Atribuir dispositivos ao público-alvo da implantação

Depois que uma implantação é criada, você pode atribuir dispositivos ao [público-alvo da implantação](/graph/api/resources/windowsupdates-deploymentaudience). Quando o público-alvo da implantação é atualizado com êxito, o Windows Update começa a oferecer a atualização para os dispositivos relevantes de acordo com as configurações de implantação.

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

Depois que todos os dispositivos atribuídos a um público de implantação tiverem sido inicialmente oferecidos à atualização, é possível que nem todos os dispositivos tenham iniciado ou concluído a atualização, devido a fatores como a conectividade do dispositivo. Desde que a implantação ainda exista, ela continuará a garantir que o Windows Update esteja oferecendo a atualização aos dispositivos atribuídos sempre que eles se reconectarem.
