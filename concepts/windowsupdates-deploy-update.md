---
title: Implantar uma atualização de recurso usando o serviço de implantação Windows Atualização para Empresas
description: Com o Windows de implantação do Update for Business, você pode implantar Windows de recursos em dispositivos em um locatário do Azure AD.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 2022294dc9467c2854642ac255169aa867ac162e
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151598"
---
# <a name="deploy-a-feature-update-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="9fe94-103">Implantar uma atualização de recurso usando o serviço de implantação Windows Atualização para Empresas</span><span class="sxs-lookup"><span data-stu-id="9fe94-103">Deploy a feature update using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="9fe94-104">Com o Windows de implantação do Update for Business, você pode implantar Windows atualizações em dispositivos em um locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9fe94-104">With the Windows Update for Business deployment service, you can deploy Windows updates to devices in an Azure AD tenant.</span></span> <span data-ttu-id="9fe94-105">Hoje, o serviço de implantação oferece suporte a [implantações](windowsupdates-deployments.md) de Windows 10 de recursos e atualizações de segurança rápidas.</span><span class="sxs-lookup"><span data-stu-id="9fe94-105">Today, the deployment service supports [deployments](windowsupdates-deployments.md) of Windows 10 feature updates and expedited security updates.</span></span> <span data-ttu-id="9fe94-106">Este tópico se concentra em implantações de atualizações de recursos.</span><span class="sxs-lookup"><span data-stu-id="9fe94-106">This topic focuses on deployments of feature updates.</span></span> <span data-ttu-id="9fe94-107">Para obter informações sobre como implantar atualizações de segurança aceleradas, consulte [Deploy an expedited security update](windowsupdates-deploy-expedited-update.md).</span><span class="sxs-lookup"><span data-stu-id="9fe94-107">For information on deploying expedited security updates, see [Deploy an expedited security update](windowsupdates-deploy-expedited-update.md).</span></span>

<span data-ttu-id="9fe94-108">Quando você implanta uma atualização de recurso em um dispositivo, o Windows Update oferece a atualização especificada para o dispositivo se ainda não tiver recebido a atualização.</span><span class="sxs-lookup"><span data-stu-id="9fe94-108">When you deploy a feature update to a device, Windows Update offers the specified update to the device if it has not yet received the update.</span></span> <span data-ttu-id="9fe94-109">Por exemplo, se você implantar Windows 10 versão 20H2 de atualização de recursos em um dispositivo que está inscrito no gerenciamento de atualização de recursos e está atualmente em uma versão mais antiga do Windows 10, o dispositivo será atualizado para a versão 20H2.</span><span class="sxs-lookup"><span data-stu-id="9fe94-109">For example, if you deploy Windows 10 feature update version 20H2 to a device that is enrolled in feature update management and is currently on an older version of Windows 10, the device updates to version 20H2.</span></span> <span data-ttu-id="9fe94-110">Se o dispositivo já estiver na versão 20H2 ou superior, ele permanecerá em sua versão atual.</span><span class="sxs-lookup"><span data-stu-id="9fe94-110">If the device is already at or above version 20H2, it stays on its current version.</span></span> <span data-ttu-id="9fe94-111">Se o dispositivo não estiver inscrito no gerenciamento de atualização de recursos, o dispositivo não será afetado por essa operação.</span><span class="sxs-lookup"><span data-stu-id="9fe94-111">If the device is not enrolled in feature update management, the device is not affected by this operation.</span></span>

<span data-ttu-id="9fe94-112">Enquanto um dispositivo permanecer inscrito no gerenciamento de atualização de recursos, o dispositivo não receberá outras atualizações de recursos do Windows Update, a menos que seja implantado explicitamente usando o serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="9fe94-112">As long as a device remains enrolled in feature update management, the device does not receive any other feature updates from Windows Update unless explicitly deployed using the deployment service.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fe94-113">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9fe94-113">Prerequisites</span></span>

* <span data-ttu-id="9fe94-114">Os dispositivos [atendem aos pré-requisitos do serviço de implantação](windowsupdates-concept-overview.md#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="9fe94-114">Devices meet the [prerequisites for the deployment service](windowsupdates-concept-overview.md#prerequisites).</span></span>
* <span data-ttu-id="9fe94-115">Antes de usar o serviço de implantação para [](windowsupdates-enroll.md) implantar atualizações de recursos, os dispositivos devem estar inscritos no gerenciamento pelo serviço de implantação para a categoria de atualização de recursos.</span><span class="sxs-lookup"><span data-stu-id="9fe94-115">Before you can use the deployment service to deploy feature updates, devices must be [enrolled in management](windowsupdates-enroll.md) by the deployment service for the feature update category.</span></span>

## <a name="step-1-optional-get-a-list-of-deployable-updates"></a><span data-ttu-id="9fe94-116">Etapa 1: (Opcional) Obter uma lista de atualizações implantáveis</span><span class="sxs-lookup"><span data-stu-id="9fe94-116">Step 1: (Optional) Get a list of deployable updates</span></span>

<span data-ttu-id="9fe94-117">Você pode consultar o catálogo de serviços de implantação para obter uma lista de atualizações que podem ser implantadas em dispositivos como conteúdo em uma implantação.</span><span class="sxs-lookup"><span data-stu-id="9fe94-117">You can query the deployment service catalog to get a list of updates that can be deployed to devices as content in a deployment.</span></span>

<span data-ttu-id="9fe94-118">Veja a seguir um exemplo de consulta para todas as Windows 10 de recursos que podem ser implantadas pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="9fe94-118">Below is an example of querying for all Windows 10 feature updates that are deployable by the deployment service.</span></span>

### <a name="request"></a><span data-ttu-id="9fe94-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fe94-119">Request</span></span>

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$filter=isof('microsoft.graph.windowsUpdates.featureUpdateCatalogEntry')
```

### <a name="response"></a><span data-ttu-id="9fe94-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fe94-120">Response</span></span>

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

## <a name="step-2-create-a-deployment"></a><span data-ttu-id="9fe94-121">Etapa 2: Criar uma implantação</span><span class="sxs-lookup"><span data-stu-id="9fe94-121">Step 2: Create a deployment</span></span>

<span data-ttu-id="9fe94-122">Uma [implantação](/graph/api/resources/windowsupdates-deployment) especifica o conteúdo a ser implantado, como e quando implantar o conteúdo e os dispositivos direcionados.</span><span class="sxs-lookup"><span data-stu-id="9fe94-122">A [deployment](/graph/api/resources/windowsupdates-deployment) specifies content to deploy, how and when to deploy the content, and the targeted devices.</span></span> <span data-ttu-id="9fe94-123">Quando uma implantação é criada, uma audiência de implantação é criada automaticamente como uma relação.</span><span class="sxs-lookup"><span data-stu-id="9fe94-123">When a deployment is created, a deployment audience is automatically created as a relationship.</span></span>

<span data-ttu-id="9fe94-124">A seguir está um exemplo de criação de uma implantação de uma atualização de recursos, com configurações opcionais configurando o [cronograma](windowsupdates-schedule-deployment.md) de implantação e as regras [de monitoramento.](windowsupdates-manage-monitoring-rules.md)</span><span class="sxs-lookup"><span data-stu-id="9fe94-124">Below is an example of creating a deployment of a feature update, with optional settings configuring the [deployment schedule](windowsupdates-schedule-deployment.md) and [monitoring rules](windowsupdates-manage-monitoring-rules.md).</span></span> <span data-ttu-id="9fe94-125">Os dispositivos direcionados são especificados na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="9fe94-125">The targeted devices are specified in the next step.</span></span>

> [!NOTE]
> <span data-ttu-id="9fe94-126">Se você não especificar uma regra [de monitoramento](/graph/api/resources/windowsupdates-monitoringrule) ao criar uma implantação, uma regra de monitoramento padrão será criada.</span><span class="sxs-lookup"><span data-stu-id="9fe94-126">If you do not specify a [monitoring rule](/graph/api/resources/windowsupdates-monitoringrule) when creating a deployment, a default monitoring rule is created.</span></span> <span data-ttu-id="9fe94-127">Esta regra de monitoramento padrão tem **um sinal** de , `rollback` um **limite** de e `20` uma **ação** de `alertError` .</span><span class="sxs-lookup"><span data-stu-id="9fe94-127">This default monitoring rule has a **signal** of `rollback`, a **threshold** of `20`, and an **action** of `alertError`.</span></span> <span data-ttu-id="9fe94-128">Em uma atualização futura da API, esse comportamento mudará e uma regra de monitoramento padrão não será criada.</span><span class="sxs-lookup"><span data-stu-id="9fe94-128">In a future update of the API, this behavior will change and a default monitoring rule will not be created.</span></span>

### <a name="request"></a><span data-ttu-id="9fe94-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fe94-129">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="9fe94-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fe94-130">Response</span></span>

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

## <a name="step-3-assign-devices-to-the-deployment-audience"></a><span data-ttu-id="9fe94-131">Etapa 3: Atribuir dispositivos à audiência de implantação</span><span class="sxs-lookup"><span data-stu-id="9fe94-131">Step 3: Assign devices to the deployment audience</span></span>

<span data-ttu-id="9fe94-132">Após a criação de uma implantação, você pode atribuir dispositivos à audiência [de implantação.](/graph/api/resources/windowsupdates-deploymentaudience)</span><span class="sxs-lookup"><span data-stu-id="9fe94-132">After a deployment is created, you can assign devices to the [deployment audience](/graph/api/resources/windowsupdates-deploymentaudience).</span></span> <span data-ttu-id="9fe94-133">Depois que o público de implantação é atualizado com êxito, o Windows Update começa a oferecer a atualização para os dispositivos relevantes de acordo com as configurações de implantação.</span><span class="sxs-lookup"><span data-stu-id="9fe94-133">After the deployment audience is successfully updated, Windows Update starts offering the update to the relevant devices according to the deployment settings.</span></span>

<span data-ttu-id="9fe94-134">Os dispositivos são registrados automaticamente com o serviço quando adicionados aos membros ou coleções de exclusões de um público de implantação (ou seja, um [objeto azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) é criado automaticamente se ainda não existir).</span><span class="sxs-lookup"><span data-stu-id="9fe94-134">Devices are automatically registered with the service when added to the members or exclusions collections of a deployment audience (that is, an [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) object is automatically created if it does not already exist).</span></span>

<span data-ttu-id="9fe94-135">O exemplo a seguir mostra como adicionar dispositivos do Azure AD como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="9fe94-135">The follwoing example shows how to add Azure AD devices as members of the deployment audience.</span></span>

### <a name="request"></a><span data-ttu-id="9fe94-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fe94-136">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="9fe94-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fe94-137">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

## <a name="during-a-deployment"></a><span data-ttu-id="9fe94-138">Durante uma implantação</span><span class="sxs-lookup"><span data-stu-id="9fe94-138">During a deployment</span></span>

<span data-ttu-id="9fe94-139">Enquanto uma implantação está em andamento, você pode pausar a implantação atualizando seu estado **,** bem como atualizar seus membros de audiência e exclusões.</span><span class="sxs-lookup"><span data-stu-id="9fe94-139">While a deployment is in progress, you can pause the deployment by updating its **state**, as well as update its audience members and exclusions.</span></span>

## <a name="after-a-deployment"></a><span data-ttu-id="9fe94-140">Após uma implantação</span><span class="sxs-lookup"><span data-stu-id="9fe94-140">After a deployment</span></span>

<span data-ttu-id="9fe94-141">Depois que todos os dispositivos atribuídos a um público de implantação foram inicialmente oferecidos a atualização, é possível que nem todos os dispositivos tenham iniciado ou concluído a atualização, devido a fatores como a conectividade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9fe94-141">After all devices assigned to a deployment audience have been initially offered the update, it is possible that not all devices have started or completed the update, due to factors like device connectivity.</span></span> <span data-ttu-id="9fe94-142">Enquanto a implantação ainda existir, o Windows Update continuará a oferecer a atualização para os dispositivos atribuídos sempre que eles se reconectam.</span><span class="sxs-lookup"><span data-stu-id="9fe94-142">As long as the deployment still exists, Windows Update continues to offer the update to the assigned devices whenever they reconnect.</span></span>

