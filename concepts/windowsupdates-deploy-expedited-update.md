---
title: Implantar uma atualização de segurança acelerada usando o serviço de implantação Windows Update for Business
description: Com o serviço de implantação do Windows Update for Business, você pode implantar atualizações de segurança Windows em dispositivos em um locatário do Azure AD caso surja uma emergência e você precise implantar imediatamente uma atualização de segurança.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: d64cb09545d1ce664b017ba3fcbcd5989d0f2a25
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210189"
---
# <a name="deploy-an-expedited-security-update-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="fc002-103">Implantar uma atualização de segurança acelerada usando o serviço de implantação Windows Update for Business</span><span class="sxs-lookup"><span data-stu-id="fc002-103">Deploy an expedited security update using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="fc002-104">Com o Windows de implantação do Update for Business, você pode implantar Windows atualizações em dispositivos em um locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fc002-104">With the Windows Update for Business deployment service, you can deploy Windows updates to devices in an Azure AD tenant.</span></span> <span data-ttu-id="fc002-105">Hoje, o serviço de implantação oferece suporte a [implantações](windowsupdates-deployments.md) de Windows 10 de recursos e atualizações de segurança rápidas.</span><span class="sxs-lookup"><span data-stu-id="fc002-105">Today, the deployment service supports [deployments](windowsupdates-deployments.md) of Windows 10 feature updates and expedited security updates.</span></span> <span data-ttu-id="fc002-106">Este tópico se concentra em implantações de atualizações de segurança aceleradas.</span><span class="sxs-lookup"><span data-stu-id="fc002-106">This topic focuses on deployments of expedited security updates.</span></span> <span data-ttu-id="fc002-107">Para obter informações sobre como implantar atualizações de recursos, consulte [Deploy a feature update](windowsupdates-deploy-update.md).</span><span class="sxs-lookup"><span data-stu-id="fc002-107">For information on deploying feature updates, see [Deploy a feature update](windowsupdates-deploy-update.md).</span></span>

<span data-ttu-id="fc002-108">Agilizar uma atualização de segurança substitui Windows políticas de adiamento do Update for Business para que a atualização seja instalada o mais rápido possível.</span><span class="sxs-lookup"><span data-stu-id="fc002-108">Expediting a security update overrides Windows Update for Business deferral policies so that the update is installed as quickly as possible.</span></span> <span data-ttu-id="fc002-109">Ele pode ser útil quando surgirem eventos críticos de segurança e você precisar implantar as atualizações mais recentes mais rapidamente do que o normal.</span><span class="sxs-lookup"><span data-stu-id="fc002-109">It can be useful when critical security events arise and you need to deploy the latest updates more rapidly than normal.</span></span> <span data-ttu-id="fc002-110">No entanto, embora possa ajudar a atingir metas de conformidade em relação a uma atualização de segurança específica, ela não foi projetada para ser usada todos os meses.</span><span class="sxs-lookup"><span data-stu-id="fc002-110">However, while it can help to achieve compliance targets against a specific security update, it is not designed to be used every month.</span></span> <span data-ttu-id="fc002-111">Em vez disso, considere o [uso de prazos de conformidade para atualizações.](https://docs.microsoft.com/windows/deployment/update/wufb-compliancedeadlines)</span><span class="sxs-lookup"><span data-stu-id="fc002-111">Instead, consider using [compliance deadlines for updates](https://docs.microsoft.com/windows/deployment/update/wufb-compliancedeadlines).</span></span>

<span data-ttu-id="fc002-112">Quando você implanta uma atualização de segurança acelerada em um dispositivo, o Windows Update oferece a atualização aplicável mais recente ao dispositivo se ainda não tiver recebido a atualização com a data de lançamento especificada.</span><span class="sxs-lookup"><span data-stu-id="fc002-112">When you deploy an expedited security update to a device, Windows Update offers the latest applicable update to the device if it has not yet received the update with the specified release date.</span></span> <span data-ttu-id="fc002-113">Por exemplo, se você implantar a atualização de segurança Windows 10 lançada em 13 de abril de 2021 em um dispositivo que não tenha a atualização no momento, o dispositivo receberá uma atualização acelerada.</span><span class="sxs-lookup"><span data-stu-id="fc002-113">For example, if you deploy the Windows 10 security update released on April 13, 2021 to a device that does not currently have the update, the device receives an expedited update.</span></span> <span data-ttu-id="fc002-114">Se o dispositivo já tiver a atualização especificada ou mais recente, ele não receberá uma atualização acelerada.</span><span class="sxs-lookup"><span data-stu-id="fc002-114">If the device already has the specified update or newer, it does not receive an expedited update.</span></span>

<span data-ttu-id="fc002-115">Atualizações de segurança aceleradas também têm as seguintes características:</span><span class="sxs-lookup"><span data-stu-id="fc002-115">Expedited security updates also have the following characteristics:</span></span>

* <span data-ttu-id="fc002-116">A atualização começa imediatamente, em vez de aguardar a próxima verificação de atualização regular, que ocorre uma vez a cada 22 horas por padrão.</span><span class="sxs-lookup"><span data-stu-id="fc002-116">The update starts right away rather than waiting for the next regular update scan, which occurs once every 22 hours by default.</span></span>
* <span data-ttu-id="fc002-117">A atualização baixa e instala o mais rápido possível.</span><span class="sxs-lookup"><span data-stu-id="fc002-117">The update downloads and installs as quickly as possible.</span></span>
* <span data-ttu-id="fc002-118">O processo de atualização substitui configurações de política de dispositivo, como dias até que o dispositivo seja forçado a reiniciar.</span><span class="sxs-lookup"><span data-stu-id="fc002-118">The update process overrides configured device policy settings, such as days until the device is forced to restart.</span></span> <span data-ttu-id="fc002-119">Depois que a atualização acelerada é instalada, o dispositivo retorna às configurações de política atuais.</span><span class="sxs-lookup"><span data-stu-id="fc002-119">After the expedited update is installed, the device returns to the current policy settings.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc002-120">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc002-120">Prerequisites</span></span>

* <span data-ttu-id="fc002-121">Os dispositivos [atendem aos pré-requisitos do serviço de implantação](windowsupdates-concept-overview.md#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="fc002-121">Devices meet the [prerequisites for the deployment service](windowsupdates-concept-overview.md#prerequisites).</span></span>
* <span data-ttu-id="fc002-122">Os dispositivos instalaram a atualização descrita em [KB4023057 Windows 10 -](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a) Atualização para componentes do Serviço de Atualização (ou mais recente).</span><span class="sxs-lookup"><span data-stu-id="fc002-122">Devices have installed the update described in [KB4023057 - Update for Windows 10 Update Service components](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a) (or newer).</span></span>

## <a name="step-1-optional-get-a-list-of-expeditable-updates"></a><span data-ttu-id="fc002-123">Etapa 1: (Opcional) Obter uma lista de atualizações de conveniência</span><span class="sxs-lookup"><span data-stu-id="fc002-123">Step 1: (Optional) Get a list of expeditable updates</span></span>

<span data-ttu-id="fc002-124">Você pode consultar o catálogo de serviços de implantação para obter uma lista de atualizações que podem ser aceleradas para dispositivos como conteúdo em uma implantação.</span><span class="sxs-lookup"><span data-stu-id="fc002-124">You can query the deployment service catalog to get a list of updates that can be expedited to devices as content in a deployment.</span></span>

<span data-ttu-id="fc002-125">As atualizações de segurança são representadas pelo [tipo qualityUpdateCatalogEntry,](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) com **uma qualityUpdateClassification** de `security` .</span><span class="sxs-lookup"><span data-stu-id="fc002-125">Security updates are represented by the [qualityUpdateCatalogEntry](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) type, with a **qualityUpdateClassification** of `security`.</span></span> <span data-ttu-id="fc002-126">Todas Windows 10 de qualidade classificadas como atualizações de segurança podem ser aceleradas e marcadas com a **propriedade isExpeditable** definida para `true` identificá-las.</span><span class="sxs-lookup"><span data-stu-id="fc002-126">All Windows 10 quality updates that are classified as security updates can be expedited and are tagged with the **isExpeditable** property set to `true` to identify them.</span></span>

<span data-ttu-id="fc002-127">Veja a seguir um exemplo de consulta para todas as Windows 10 de segurança que podem ser implantadas como atualizações aceleradas pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="fc002-127">Below is an example of querying for all Windows 10 security updates that can be deployed as expedited updates by the deployment service.</span></span> <span data-ttu-id="fc002-128">A Microsoft recomenda mostrar apenas as três atualizações mais atuais, portanto, o exemplo inclui `$top=3` .</span><span class="sxs-lookup"><span data-stu-id="fc002-128">Microsoft recommends to only show the three most current updates, so the example includes `$top=3`.</span></span>

### <a name="request"></a><span data-ttu-id="fc002-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc002-129">Request</span></span>

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$top=3&$filter=isof('microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry') and microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry/isExpeditable eq true&$orderby=releaseDateTime desc
```

### <a name="response"></a><span data-ttu-id="fc002-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc002-130">Response</span></span>

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

## <a name="step-2-create-a-deployment"></a><span data-ttu-id="fc002-131">Etapa 2: Criar uma implantação</span><span class="sxs-lookup"><span data-stu-id="fc002-131">Step 2: Create a deployment</span></span>

<span data-ttu-id="fc002-132">Uma [implantação](/graph/api/resources/windowsupdates-deployment) especifica o conteúdo a ser implantado, como e quando implantar o conteúdo e os dispositivos direcionados.</span><span class="sxs-lookup"><span data-stu-id="fc002-132">A [deployment](/graph/api/resources/windowsupdates-deployment) specifies content to deploy, how and when to deploy the content, and the targeted devices.</span></span> <span data-ttu-id="fc002-133">Para atualizações de qualidade, o conteúdo é especificado usando uma data de conformidade de destino.</span><span class="sxs-lookup"><span data-stu-id="fc002-133">For quality updates, the content is specified using a target compliance date.</span></span> <span data-ttu-id="fc002-134">Quando uma implantação é criada, uma audiência de implantação é criada automaticamente como uma relação.</span><span class="sxs-lookup"><span data-stu-id="fc002-134">When a deployment is created, a deployment audience is automatically created as a relationship.</span></span>

<span data-ttu-id="fc002-135">Quando você implanta uma atualização de segurança acelerada em um dispositivo, o Windows Update oferece uma atualização que traz o dispositivo acima do nível mínimo de conformidade especificado.</span><span class="sxs-lookup"><span data-stu-id="fc002-135">When you deploy an expedited security update to a device, Windows Update offers an update that brings the device above the minimum compliance level specified.</span></span> <span data-ttu-id="fc002-136">Dependendo de quando cada dispositivo verifica e atualiza, alguns dispositivos podem receber atualizações mais novas (por exemplo, se houver uma atualização de segurança mais recente do que a correspondente ao nível mínimo de conformidade desejado), mas todos os dispositivos atendem ao padrão de conformidade de atualização de segurança especificado.</span><span class="sxs-lookup"><span data-stu-id="fc002-136">Depending on when each device scans and updates, some devices may receive newer updates (e.g. if there is a newer security update than the one corresponding to the desired minimum compliance level), but all devices meet the specified security update compliance standard.</span></span> <span data-ttu-id="fc002-137">Esse comportamento de oferecer a atualização aplicável mais recente, indicada pela propriedade **equivalentContent** que está sendo definida como o valor padrão, ajuda a manter os dispositivos o mais seguros possível e impede que um dispositivo receba uma atualização acelerada seguida por outra atualização regular apenas dias `latestSecurity` depois.</span><span class="sxs-lookup"><span data-stu-id="fc002-137">This behavior of offering the latest applicable update, indicated by the property **equivalentContent** being set to the default value `latestSecurity`, helps keep devices as secure as possible and prevents a device from receiving an expedited update followed by another regular update just days later.</span></span>

<span data-ttu-id="fc002-138">Você pode configurar o período de carência de reinicialização do dispositivo usando os dias da **propriedadeUntilForcedReboot** nas configurações de experiência [do](/graph/api/resources/windowsupdates-userexperiencesettings) usuário da implantação.</span><span class="sxs-lookup"><span data-stu-id="fc002-138">You can configure the device restart grace period using the property **daysUntilForcedReboot** in the [user experience settings](/graph/api/resources/windowsupdates-userexperiencesettings) of the deployment.</span></span> <span data-ttu-id="fc002-139">O período de carência define a quantidade de tempo após a instalação que o usuário pode controlar o tempo de quando o dispositivo é reiniciado.</span><span class="sxs-lookup"><span data-stu-id="fc002-139">The grace period sets the amount of time after installation that the user can control the timing of when the device restarts.</span></span> <span data-ttu-id="fc002-140">Se o dispositivo não tiver reiniciado quando o período de carência expirar, ele será reiniciado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="fc002-140">If the device has not restarted by the time the grace period expires, it restarts automatically.</span></span>

<span data-ttu-id="fc002-141">A seguir está um exemplo de criação de uma implantação para uma atualização de qualidade acelerada.</span><span class="sxs-lookup"><span data-stu-id="fc002-141">Below is an example of creating a deployment for an expedited quality update.</span></span> <span data-ttu-id="fc002-142">Os dispositivos direcionados são especificados na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="fc002-142">The targeted devices are specified in the next step.</span></span>

### <a name="request"></a><span data-ttu-id="fc002-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc002-143">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="fc002-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc002-144">Response</span></span>

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

## <a name="step-3-assign-devices-to-the-deployment-audience"></a><span data-ttu-id="fc002-145">Etapa 3: Atribuir dispositivos à audiência de implantação</span><span class="sxs-lookup"><span data-stu-id="fc002-145">Step 3: Assign devices to the deployment audience</span></span>

<span data-ttu-id="fc002-146">Após a criação de uma implantação, você pode atribuir dispositivos à audiência [de implantação.](/graph/api/resources/windowsupdates-deploymentaudience)</span><span class="sxs-lookup"><span data-stu-id="fc002-146">After a deployment is created, you can assign devices to the [deployment audience](/graph/api/resources/windowsupdates-deploymentaudience).</span></span> <span data-ttu-id="fc002-147">Quando o público de implantação é atualizado com êxito, o Windows Update começa a oferecer a atualização para os dispositivos relevantes de acordo com as configurações de implantação.</span><span class="sxs-lookup"><span data-stu-id="fc002-147">When the deployment audience is successfully updated, Windows Update starts offering the update to the relevant devices according to the deployment settings.</span></span>

<span data-ttu-id="fc002-148">Os dispositivos são registrados automaticamente com o serviço quando adicionados aos membros ou coleções de exclusões de um público de implantação (ou seja, um [objeto azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) é criado automaticamente se ainda não existir).</span><span class="sxs-lookup"><span data-stu-id="fc002-148">Devices are automatically registered with the service when added to the members or exclusions collections of a deployment audience (that is, an [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) object is automatically created if it does not already exist).</span></span>

<span data-ttu-id="fc002-149">O exemplo a seguir mostra como adicionar dispositivos do Azure AD como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="fc002-149">The following example shows how to add Azure AD devices as members of the deployment audience.</span></span>

### <a name="request"></a><span data-ttu-id="fc002-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc002-150">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="fc002-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc002-151">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

## <a name="during-a-deployment"></a><span data-ttu-id="fc002-152">Durante uma implantação</span><span class="sxs-lookup"><span data-stu-id="fc002-152">During a deployment</span></span>

<span data-ttu-id="fc002-153">Enquanto uma implantação está em andamento, você pode pausar a implantação atualizando seu estado **,** bem como atualizar seus membros de audiência e exclusões.</span><span class="sxs-lookup"><span data-stu-id="fc002-153">While a deployment is in progress, you can pause the deployment by updating its **state**, as well as update its audience members and exclusions.</span></span>

## <a name="after-a-deployment"></a><span data-ttu-id="fc002-154">Após uma implantação</span><span class="sxs-lookup"><span data-stu-id="fc002-154">After a deployment</span></span>

<span data-ttu-id="fc002-155">Depois que todos os dispositivos atribuídos a um público de implantação foram inicialmente oferecidos a atualização, é possível que nem todos os dispositivos tenham iniciado ou concluído a atualização, devido a fatores como a conectividade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fc002-155">After all devices assigned to a deployment audience have been initially offered the update, it is possible that not all devices have started or completed the update, due to factors like device connectivity.</span></span> <span data-ttu-id="fc002-156">Enquanto a implantação ainda existir, ela continuará a garantir que o Windows Update esteja oferecendo a atualização para os dispositivos atribuídos sempre que eles se reconectam.</span><span class="sxs-lookup"><span data-stu-id="fc002-156">As long as the deployment still exists, it continues to make sure that Windows Update is offering the update to the assigned devices whenever they reconnect.</span></span>
