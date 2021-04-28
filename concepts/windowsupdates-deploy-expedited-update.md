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
# <a name="deploy-an-expedited-security-update-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="8ae80-103">Implantar uma atualização de segurança acelerada usando o serviço de implantação Windows Update for Business</span><span class="sxs-lookup"><span data-stu-id="8ae80-103">Deploy an expedited security update using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="8ae80-104">Com o Windows de implantação do Update for Business, você pode implantar Windows atualizações em dispositivos em um locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8ae80-104">With the Windows Update for Business deployment service, you can deploy Windows updates to devices in an Azure AD tenant.</span></span> <span data-ttu-id="8ae80-105">Hoje, o serviço de implantação oferece suporte a [implantações](windowsupdates-deployments.md) de Windows 10 de recursos e atualizações de segurança rápidas.</span><span class="sxs-lookup"><span data-stu-id="8ae80-105">Today, the deployment service supports [deployments](windowsupdates-deployments.md) of Windows 10 feature updates and expedited security updates.</span></span> <span data-ttu-id="8ae80-106">Este tópico se concentra em implantações de atualizações de segurança aceleradas.</span><span class="sxs-lookup"><span data-stu-id="8ae80-106">This topic focuses on deployments of expedited security updates.</span></span> <span data-ttu-id="8ae80-107">Para obter informações sobre como implantar atualizações de recursos, consulte [Deploy a feature update](windowsupdates-deploy-update.md).</span><span class="sxs-lookup"><span data-stu-id="8ae80-107">For information on deploying feature updates, see [Deploy a feature update](windowsupdates-deploy-update.md).</span></span>

<span data-ttu-id="8ae80-108">Agilizar uma atualização de segurança substitui Windows políticas de adiamento do Update for Business para que a atualização seja instalada o mais rápido possível.</span><span class="sxs-lookup"><span data-stu-id="8ae80-108">Expediting a security update overrides Windows Update for Business deferral policies so that the update is installed as quickly as possible.</span></span> <span data-ttu-id="8ae80-109">Ele pode ser útil quando surgirem eventos críticos de segurança e você precisar implantar as atualizações mais recentes mais rapidamente do que o normal.</span><span class="sxs-lookup"><span data-stu-id="8ae80-109">It can be useful when critical security events arise and you need to deploy the latest updates more rapidly than normal.</span></span> <span data-ttu-id="8ae80-110">No entanto, embora possa ajudar a atingir metas de conformidade em relação a uma atualização de segurança específica, ela não foi projetada para ser usada todos os meses.</span><span class="sxs-lookup"><span data-stu-id="8ae80-110">However, while it can help to achieve compliance targets against a specific security update, it is not designed to be used every month.</span></span> <span data-ttu-id="8ae80-111">Em vez disso, considere o [uso de prazos de conformidade para atualizações.](https://docs.microsoft.com/windows/deployment/update/wufb-compliancedeadlines)</span><span class="sxs-lookup"><span data-stu-id="8ae80-111">Instead, consider using [compliance deadlines for updates](https://docs.microsoft.com/windows/deployment/update/wufb-compliancedeadlines).</span></span>

<span data-ttu-id="8ae80-112">Quando você implanta uma atualização de segurança acelerada em um dispositivo, o Windows Update oferece a atualização aplicável mais recente ao dispositivo se ainda não tiver recebido a atualização com a data de lançamento especificada.</span><span class="sxs-lookup"><span data-stu-id="8ae80-112">When you deploy an expedited security update to a device, Windows Update offers the latest applicable update to the device if it has not yet received the update with the specified release date.</span></span> <span data-ttu-id="8ae80-113">Por exemplo, se você implantar a atualização de segurança Windows 10 lançada em 13 de abril de 2021 em um dispositivo que não tenha a atualização no momento, o dispositivo receberá uma atualização acelerada.</span><span class="sxs-lookup"><span data-stu-id="8ae80-113">For example, if you deploy the Windows 10 security update released on April 13, 2021 to a device that does not currently have the update, the device receives an expedited update.</span></span> <span data-ttu-id="8ae80-114">Se o dispositivo já tiver a atualização especificada ou mais recente, ele não receberá uma atualização acelerada.</span><span class="sxs-lookup"><span data-stu-id="8ae80-114">If the device already has the specified update or newer, it does not receive an expedited update.</span></span>

<span data-ttu-id="8ae80-115">Atualizações de segurança aceleradas também têm as seguintes características:</span><span class="sxs-lookup"><span data-stu-id="8ae80-115">Expedited security updates also have the following characteristics:</span></span>

* <span data-ttu-id="8ae80-116">A atualização começa imediatamente, em vez de aguardar a próxima verificação de atualização regular, que ocorre uma vez a cada 22 horas por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ae80-116">The update starts right away rather than waiting for the next regular update scan, which occurs once every 22 hours by default.</span></span>
* <span data-ttu-id="8ae80-117">A atualização baixa e instala o mais rápido possível.</span><span class="sxs-lookup"><span data-stu-id="8ae80-117">The update downloads and installs as quickly as possible.</span></span>
* <span data-ttu-id="8ae80-118">O processo de atualização substitui configurações de política de dispositivo, como dias até que o dispositivo seja forçado a reiniciar.</span><span class="sxs-lookup"><span data-stu-id="8ae80-118">The update process overrides configured device policy settings, such as days until the device is forced to restart.</span></span> <span data-ttu-id="8ae80-119">Depois que a atualização acelerada é instalada, o dispositivo retorna às configurações de política atuais.</span><span class="sxs-lookup"><span data-stu-id="8ae80-119">After the expedited update is installed, the device returns to the current policy settings.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ae80-120">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ae80-120">Prerequisites</span></span>

* <span data-ttu-id="8ae80-121">Os dispositivos [atendem aos pré-requisitos do serviço de implantação](windowsupdates-concept-overview.md#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="8ae80-121">Devices meet the [prerequisites for the deployment service](windowsupdates-concept-overview.md#prerequisites).</span></span>
* <span data-ttu-id="8ae80-122">Os dispositivos instalaram a atualização descrita em [KB4023057 Windows 10 -](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a) Atualização para componentes do Serviço de Atualização (ou mais recente).</span><span class="sxs-lookup"><span data-stu-id="8ae80-122">Devices have installed the update described in [KB4023057 - Update for Windows 10 Update Service components](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a) (or newer).</span></span>

## <a name="step-1-optional-get-a-list-of-expeditable-updates"></a><span data-ttu-id="8ae80-123">Etapa 1: (Opcional) Obter uma lista de atualizações de conveniência</span><span class="sxs-lookup"><span data-stu-id="8ae80-123">Step 1: (Optional) Get a list of expeditable updates</span></span>

<span data-ttu-id="8ae80-124">Você pode consultar o catálogo de serviços de implantação para obter uma lista de atualizações que podem ser aceleradas para dispositivos como conteúdo em uma implantação.</span><span class="sxs-lookup"><span data-stu-id="8ae80-124">You can query the deployment service catalog to get a list of updates that can be expedited to devices as content in a deployment.</span></span>

<span data-ttu-id="8ae80-125">As atualizações de segurança são representadas pelo [tipo qualityUpdateCatalogEntry,](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) com **uma qualityUpdateClassification** de `security` .</span><span class="sxs-lookup"><span data-stu-id="8ae80-125">Security updates are represented by the [qualityUpdateCatalogEntry](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) type, with a **qualityUpdateClassification** of `security`.</span></span> <span data-ttu-id="8ae80-126">Todas Windows 10 de qualidade classificadas como atualizações de segurança podem ser aceleradas e marcadas com a **propriedade isExpeditable** definida para `true` identificá-las.</span><span class="sxs-lookup"><span data-stu-id="8ae80-126">All Windows 10 quality updates that are classified as security updates can be expedited and are tagged with the **isExpeditable** property set to `true` to identify them.</span></span>

<span data-ttu-id="8ae80-127">Veja a seguir um exemplo de consulta para todas as Windows 10 de segurança que podem ser implantadas como atualizações aceleradas pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="8ae80-127">Below is an example of querying for all Windows 10 security updates that can be deployed as expedited updates by the deployment service.</span></span> <span data-ttu-id="8ae80-128">A Microsoft recomenda mostrar apenas as três atualizações mais atuais, portanto, o exemplo inclui `$top=3` .</span><span class="sxs-lookup"><span data-stu-id="8ae80-128">Microsoft recommends to only show the three most current updates, so the example includes `$top=3`.</span></span>

### <a name="request"></a><span data-ttu-id="8ae80-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ae80-129">Request</span></span>

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$top=3&$filter=isof('microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry') and microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry/isExpeditable eq true&$orderby=releaseDateTime desc
```

### <a name="response"></a><span data-ttu-id="8ae80-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ae80-130">Response</span></span>

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

## <a name="step-2-create-a-deployment"></a><span data-ttu-id="8ae80-131">Etapa 2: Criar uma implantação</span><span class="sxs-lookup"><span data-stu-id="8ae80-131">Step 2: Create a deployment</span></span>

> [!NOTE]
> <span data-ttu-id="8ae80-132">Na primeira vez que você implantar uma atualização de segurança acelerada em seu locatário, poderá ter até um atraso de um dia enquanto o serviço estiver configurado para sua organização.</span><span class="sxs-lookup"><span data-stu-id="8ae80-132">The first time you deploy an expedited security update in your tenant, you may experience up to a one-day delay while the service is configured for your organization.</span></span> <span data-ttu-id="8ae80-133">Esse atraso não se aplica a implantações ou implantações subsequentes de atualizações de recursos e será abordado em uma atualização futura.</span><span class="sxs-lookup"><span data-stu-id="8ae80-133">This delay does not apply to subsequent deployments or deployments of feature updates, and will be addressed in a future update.</span></span>

<span data-ttu-id="8ae80-134">Uma [implantação](/graph/api/resources/windowsupdates-deployment) especifica o conteúdo a ser implantado, como e quando implantar o conteúdo e os dispositivos direcionados.</span><span class="sxs-lookup"><span data-stu-id="8ae80-134">A [deployment](/graph/api/resources/windowsupdates-deployment) specifies content to deploy, how and when to deploy the content, and the targeted devices.</span></span> <span data-ttu-id="8ae80-135">Para atualizações de qualidade, o conteúdo é especificado usando uma data de conformidade de destino.</span><span class="sxs-lookup"><span data-stu-id="8ae80-135">For quality updates, the content is specified using a target compliance date.</span></span> <span data-ttu-id="8ae80-136">Quando uma implantação é criada, uma audiência de implantação é criada automaticamente como uma relação.</span><span class="sxs-lookup"><span data-stu-id="8ae80-136">When a deployment is created, a deployment audience is automatically created as a relationship.</span></span>

<span data-ttu-id="8ae80-137">Quando você implanta uma atualização de segurança acelerada em um dispositivo, o Windows Update oferece uma atualização que traz o dispositivo acima do nível mínimo de conformidade especificado.</span><span class="sxs-lookup"><span data-stu-id="8ae80-137">When you deploy an expedited security update to a device, Windows Update offers an update that brings the device above the minimum compliance level specified.</span></span> <span data-ttu-id="8ae80-138">Dependendo de quando cada dispositivo verifica e atualiza, alguns dispositivos podem receber atualizações mais novas (por exemplo, se houver uma atualização de segurança mais recente do que a correspondente ao nível mínimo de conformidade desejado), mas todos os dispositivos atendem ao padrão de conformidade de atualização de segurança especificado.</span><span class="sxs-lookup"><span data-stu-id="8ae80-138">Depending on when each device scans and updates, some devices may receive newer updates (e.g. if there is a newer security update than the one corresponding to the desired minimum compliance level), but all devices meet the specified security update compliance standard.</span></span> <span data-ttu-id="8ae80-139">Esse comportamento de oferecer a atualização aplicável mais recente, indicada pela propriedade **equivalentContent** que está sendo definida como o valor padrão, ajuda a manter os dispositivos o mais seguros possível e impede que um dispositivo receba uma atualização acelerada seguida por outra atualização regular apenas dias `latestSecurity` depois.</span><span class="sxs-lookup"><span data-stu-id="8ae80-139">This behavior of offering the latest applicable update, indicated by the property **equivalentContent** being set to the default value `latestSecurity`, helps keep devices as secure as possible and prevents a device from receiving an expedited update followed by another regular update just days later.</span></span>

<span data-ttu-id="8ae80-140">Você pode configurar o período de carência de reinicialização do dispositivo usando os dias da **propriedadeUntilForcedReboot** nas configurações de experiência [do](/graph/api/resources/windowsupdates-userexperiencesettings) usuário da implantação.</span><span class="sxs-lookup"><span data-stu-id="8ae80-140">You can configure the device restart grace period using the property **daysUntilForcedReboot** in the [user experience settings](/graph/api/resources/windowsupdates-userexperiencesettings) of the deployment.</span></span> <span data-ttu-id="8ae80-141">O período de carência define a quantidade de tempo após a instalação que o usuário pode controlar o tempo de quando o dispositivo é reiniciado.</span><span class="sxs-lookup"><span data-stu-id="8ae80-141">The grace period sets the amount of time after installation that the user can control the timing of when the device restarts.</span></span> <span data-ttu-id="8ae80-142">Se o dispositivo não tiver reiniciado quando o período de carência expirar, ele será reiniciado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="8ae80-142">If the device has not restarted by the time the grace period expires, it restarts automatically.</span></span>

<span data-ttu-id="8ae80-143">A seguir está um exemplo de criação de uma implantação para uma atualização de qualidade acelerada.</span><span class="sxs-lookup"><span data-stu-id="8ae80-143">Below is an example of creating a deployment for an expedited quality update.</span></span> <span data-ttu-id="8ae80-144">Os dispositivos direcionados são especificados na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="8ae80-144">The targeted devices are specified in the next step.</span></span>

### <a name="request"></a><span data-ttu-id="8ae80-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ae80-145">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="8ae80-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ae80-146">Response</span></span>

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

## <a name="step-3-assign-devices-to-the-deployment-audience"></a><span data-ttu-id="8ae80-147">Etapa 3: Atribuir dispositivos à audiência de implantação</span><span class="sxs-lookup"><span data-stu-id="8ae80-147">Step 3: Assign devices to the deployment audience</span></span>

<span data-ttu-id="8ae80-148">Após a criação de uma implantação, você pode atribuir dispositivos à audiência [de implantação.](/graph/api/resources/windowsupdates-deploymentaudience)</span><span class="sxs-lookup"><span data-stu-id="8ae80-148">After a deployment is created, you can assign devices to the [deployment audience](/graph/api/resources/windowsupdates-deploymentaudience).</span></span> <span data-ttu-id="8ae80-149">Os dispositivos podem ser atribuídos diretamente ou por meio de [grupos de ativos atualizáveis.](/graph/api/resources/windowsupdates-updatableassetgroup)</span><span class="sxs-lookup"><span data-stu-id="8ae80-149">Devices can be assigned directly, or via [updatable asset groups](/graph/api/resources/windowsupdates-updatableassetgroup).</span></span> <span data-ttu-id="8ae80-150">Depois que a audiência de implantação é atualizada com êxito, o Windows Update começa a oferecer a atualização para os dispositivos relevantes de acordo com as configurações de implantação.</span><span class="sxs-lookup"><span data-stu-id="8ae80-150">Once the deployment audience is successfully updated, Windows Update starts offering the update to the relevant devices according to the deployment settings.</span></span>

<span data-ttu-id="8ae80-151">Os dispositivos são registrados automaticamente com o serviço quando adicionados aos membros ou coleções de exclusões de um público de implantação (ou seja, um [objeto azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) é criado automaticamente se ainda não existir).</span><span class="sxs-lookup"><span data-stu-id="8ae80-151">Devices are automatically registered with the service when added to the members or exclusions collections of a deployment audience (i.e. an [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) object is automatically created if it does not already exist).</span></span>

<span data-ttu-id="8ae80-152">Veja a seguir um exemplo de adição de grupos de ativos atualizáveis e dispositivos do Azure AD como membros da audiência de implantação, além de excluir um dispositivo específico do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8ae80-152">Below is an example of adding updatable asset groups and Azure AD devices as members of the deployment audience, while also excluding a specific Azure AD device.</span></span>

### <a name="request"></a><span data-ttu-id="8ae80-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ae80-153">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="8ae80-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ae80-154">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

## <a name="during-a-deployment"></a><span data-ttu-id="8ae80-155">Durante uma implantação</span><span class="sxs-lookup"><span data-stu-id="8ae80-155">During a deployment</span></span>

<span data-ttu-id="8ae80-156">Enquanto uma implantação está em andamento, você pode pausar a implantação atualizando seu estado **,** bem como atualizar seus membros de audiência e exclusões.</span><span class="sxs-lookup"><span data-stu-id="8ae80-156">While a deployment is in progress, you can pause the deployment by updating its **state**, as well as update its audience members and exclusions.</span></span>

## <a name="after-a-deployment"></a><span data-ttu-id="8ae80-157">Após uma implantação</span><span class="sxs-lookup"><span data-stu-id="8ae80-157">After a deployment</span></span>

<span data-ttu-id="8ae80-158">Depois que todos os dispositivos atribuídos a um público de implantação foram inicialmente oferecidos a atualização, é possível que nem todos os dispositivos tenham iniciado ou concluído a atualização, devido a fatores como a conectividade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8ae80-158">After all devices assigned to a deployment audience have been initially offered the update, it is possible that not all devices have started or completed the update, due to factors like device connectivity.</span></span> <span data-ttu-id="8ae80-159">Enquanto a implantação ainda existir, ela continuará a garantir que o Windows Update esteja oferecendo a atualização para os dispositivos atribuídos sempre que eles se reconectam.</span><span class="sxs-lookup"><span data-stu-id="8ae80-159">As long as the deployment still exists, it continues to make sure that Windows Update is offering the update to the assigned devices whenever they reconnect.</span></span>
