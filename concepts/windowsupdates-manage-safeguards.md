---
title: Gerenciar proteções usando o serviço de implantação Windows Update for Business
description: Quando você implanta atualizações com o serviço de implantação, o serviço protege automaticamente as implantações, impedindo que dispositivos com problemas conhecidos ou prováveis de serem oferecidos a atualização pelo Windows Update.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: ff3d8c594087253db85fb943bd34fe9478f45bb9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61855516"
---
# <a name="manage-safeguards-using-the-windows-update-for-business-deployment-service"></a>Gerenciar proteções usando o serviço de implantação Windows Update for Business

Quando você implanta atualizações com o serviço de implantação, o serviço protege automaticamente as implantações, impedindo que dispositivos com problemas conhecidos ou prováveis de serem oferecidos a atualização pelo Windows Update.

As proteções são compatíveis [com implantações](windowsupdates-deployments.md) de Windows 11 e Windows 10 de recursos. Os resguardos contra problemas conhecidos estão disponíveis para implantações de atualizações de recursos do Windows 11 e Windows 10 e a proteção contra problemas prováveis estão disponíveis para implantações do Windows 11.

## <a name="apply-all-safeguards"></a>Aplicar todas as proteções

Por padrão, o serviço de implantação aplica todas as proteções aplicáveis a dispositivos em uma implantação. Para se beneficiar de proteções, você não precisa especificar nada adicional ao criar uma implantação.

O exemplo a seguir demonstra como criar uma implantação com todas as proteções aplicadas.

### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
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
    "settings": null,
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="opt-out-of-safeguards-against-likely-issues"></a>Recusar proteções contra problemas prováveis

Você pode optar por não proteger contra problemas prováveis em uma implantação configurando [configurações de proteção.](/graph/api/resources/windowsupdates-safeguardsettings) Se necessário, você também pode optar por não resguardar resguardos para problemas conhecidos [usando a política de proteções de desabilitação.](/windows/deployment/update/safeguard-opt-out)

O exemplo a seguir demonstra como criar uma implantação sem proteções contra problemas prováveis. Ao especificar um **safeguardProfile** para a categoria de na lista de perfis de proteção a desabilitar, você está configurando a implantação para oferecer a atualização a um dispositivo, mesmo que seja provável que tenha um problema de  `likelyIssues` atualização.

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
        "safeguard": {
            "disabledSafeguardProfiles": [
                {
                    "category": "likelyIssues"
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
        "monitoring": null,
        "rollout": null,
        "userExperience": null,
        "safeguard": {
            "disabledSafeguardProfiles": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.safeguardProfile",
                    "category": "likelyIssues"
                }
            ]
        }
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```
