---
title: Windows visão geral da API de atualizações
description: O Windows de implantação update for Business fornece controle à sua organização sobre as atualizações oferecidas aos seus dispositivos.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 98b75f278e33f56cf726a18c266000b06d817a6f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067653"
---
# <a name="windows-updates-api-overview"></a><span data-ttu-id="a4471-103">Windows visão geral da API de atualizações</span><span class="sxs-lookup"><span data-stu-id="a4471-103">Windows updates API overview</span></span>

<span data-ttu-id="a4471-104">O Windows de implantação update for Business fornece controle sobre as atualizações de dispositivo por meio da capacidade de aprovar, agendar e proteger o conteúdo fornecido pelo Windows Update.</span><span class="sxs-lookup"><span data-stu-id="a4471-104">The Windows Update for Business deployment service provides control over device updates through the ability to approve, schedule and safeguard content delivered by Windows Update.</span></span> 

## <a name="why-use-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="a4471-105">Por que usar o serviço de implantação Windows Atualização para Empresas?</span><span class="sxs-lookup"><span data-stu-id="a4471-105">Why use the Windows Update for Business deployment service?</span></span>

<span data-ttu-id="a4471-106">Profissionais de TI e fornecedores de ferramentas de gerenciamento podem usar o serviço de implantação para:</span><span class="sxs-lookup"><span data-stu-id="a4471-106">IT Professionals and management tool vendors alike can use the deployment service to:</span></span>
* <span data-ttu-id="a4471-107">Agendar implantações de atualização para começar em uma data específica</span><span class="sxs-lookup"><span data-stu-id="a4471-107">Schedule update deployments to begin on a specific date</span></span>
* <span data-ttu-id="a4471-108">Implantações em estágios por um período de dias ou semanas usando expressões ricas</span><span class="sxs-lookup"><span data-stu-id="a4471-108">Stage deployments over a period of days or weeks using rich expressions</span></span>
* <span data-ttu-id="a4471-109">Ignorar políticas pré-configuradas Windows Update for Business para implantar imediatamente uma atualização de segurança</span><span class="sxs-lookup"><span data-stu-id="a4471-109">Bypass pre-configured Windows Update for Business policies to immediately deploy a security update</span></span>
* <span data-ttu-id="a4471-110">Garantir a cobertura de hardware e software em sua organização por meio de implantações personalizadas para populações exclusivas de dispositivos</span><span class="sxs-lookup"><span data-stu-id="a4471-110">Ensure coverage of hardware and software in your organization through deployments tailored to unique device population(s)</span></span>

<span data-ttu-id="a4471-111">Hoje, o serviço de implantação dá suporte ao gerenciamento Windows 10 de recursos e àgilizar Windows 10 de segurança.</span><span class="sxs-lookup"><span data-stu-id="a4471-111">Today, the deployment service supports managing Windows 10 feature updates and expediting Windows 10 security updates.</span></span> <span data-ttu-id="a4471-112">Para saber mais sobre o serviço de implantação no contexto do Windows Update for Business, consulte [Overview of the deployment service](https://docs.microsoft.com/windows/deployment/update/deployment-service-overview).</span><span class="sxs-lookup"><span data-stu-id="a4471-112">To learn more about the deployment service in the context of Windows Update for Business, please see [Overview of the deployment service](https://docs.microsoft.com/windows/deployment/update/deployment-service-overview).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4471-113">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a4471-113">Prerequisites</span></span>    

<span data-ttu-id="a4471-114">Para usar o serviço de implantação, sua organização deve ter uma das seguintes assinaturas:</span><span class="sxs-lookup"><span data-stu-id="a4471-114">To use the deployment service, your organization must have one of the following subscriptions:</span></span>
* <span data-ttu-id="a4471-115">Windows 10 Enterprise E3 ou E5 (incluído no Microsoft 365 F3, E3 ou E5)</span><span class="sxs-lookup"><span data-stu-id="a4471-115">Windows 10 Enterprise E3 or E5 (included in Microsoft 365 F3, E3, or E5)</span></span>
* <span data-ttu-id="a4471-116">Windows 10 Education A3 ou A5 (incluído no Microsoft 365 A3 ou A5)</span><span class="sxs-lookup"><span data-stu-id="a4471-116">Windows 10 Education A3 or A5 (included in Microsoft 365 A3 or A5)</span></span>
* <span data-ttu-id="a4471-117">Windows Virtual Desktop Access E3 ou E5</span><span class="sxs-lookup"><span data-stu-id="a4471-117">Windows Virtual Desktop Access E3 or E5</span></span>
* <span data-ttu-id="a4471-118">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="a4471-118">Microsoft 365 Business Premium</span></span>

<span data-ttu-id="a4471-119">Além disso, os dispositivos gerenciados pelo serviço de implantação devem:</span><span class="sxs-lookup"><span data-stu-id="a4471-119">Additionally, devices managed by the deployment service must:</span></span>
* <span data-ttu-id="a4471-120">Ser ingressado no Azure AD ou Ingresso no AD Híbrido</span><span class="sxs-lookup"><span data-stu-id="a4471-120">Be Azure AD joined or Hybrid AD joined</span></span>
* <span data-ttu-id="a4471-121">Execute uma das seguintes edições Windows 10: Windows 10 Pro, Windows 10 Enterprise, Windows 10 Education, Windows 10 Pro Education</span><span class="sxs-lookup"><span data-stu-id="a4471-121">Run one of the following Windows 10 editions: Windows 10 Pro, Windows 10 Enterprise, Windows 10 Education, Windows 10 Pro Education</span></span>
* <span data-ttu-id="a4471-122">Ter instalado Windows 10 versão 1709 ou posterior</span><span class="sxs-lookup"><span data-stu-id="a4471-122">Have installed Windows 10 version 1709 or later</span></span>

## <a name="enroll-devices-to-be-managed"></a><span data-ttu-id="a4471-123">Registrar dispositivos a serem gerenciados</span><span class="sxs-lookup"><span data-stu-id="a4471-123">Enroll devices to be managed</span></span>

<span data-ttu-id="a4471-124">Para começar a usar o serviço de implantação, [inscreva dispositivos no gerenciamento de atualizações.](windowsupdates-enroll.md)</span><span class="sxs-lookup"><span data-stu-id="a4471-124">To start using the deployment service, [enroll devices in update management](windowsupdates-enroll.md).</span></span>

## <a name="approve-and-schedule-windows-content-delivered-from-windows-update"></a><span data-ttu-id="a4471-125">Aprovar e agendar Windows conteúdo entregue do Windows Update</span><span class="sxs-lookup"><span data-stu-id="a4471-125">Approve and schedule Windows content delivered from Windows Update</span></span>

<span data-ttu-id="a4471-126">O serviço de implantação simplifica a revisão, aprovação, agendamento e implantação de conteúdo para um ecossistema de dispositivos diversificado.</span><span class="sxs-lookup"><span data-stu-id="a4471-126">The deployment service simplifies reviewing, approving, scheduling, and deploying content for a diverse device ecosystem.</span></span> <span data-ttu-id="a4471-127">Existe um catálogo de atualizações para fornecer uma exibição personalizada para aprovações, ajudando você a se concentrar nas decisões de aprovação que importam e evitando a necessidade de classificar por meio de listas profundas de atualizações relacionadas.</span><span class="sxs-lookup"><span data-stu-id="a4471-127">An updates catalog exists to provide a view tailored for approvals, helping you focus on approval decisions that matter and avoiding the need to sort through deep lists of related updates.</span></span>

<span data-ttu-id="a4471-128">Depois de escolher uma atualização para implantar, você pode agendar implantações para iniciar em uma hora futura ou implantar por um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="a4471-128">Once you choose an update to deploy, you can schedule deployments to start at a future time, or deploy over a period of time.</span></span> <span data-ttu-id="a4471-129">Se você optar por implantar uma atualização por um período de tempo, o serviço de implantação otimizará automaticamente a ordem na qual os dispositivos são oferecidos atualizações.</span><span class="sxs-lookup"><span data-stu-id="a4471-129">If you choose to deploy an update over a period of time, the deployment service automatically optimizes the order in which devices are offered updates.</span></span> <span data-ttu-id="a4471-130">Quando possível, o serviço ordena dispositivos para garantir que uma diversidade de ativos de hardware e software seja representada no início da implantação para minimizar o número de dispositivos que podem encontrar um problema de atualização inesperado.</span><span class="sxs-lookup"><span data-stu-id="a4471-130">When possible, the service orders devices to ensure that a diversity of hardware and software assets are represented early in the deployment to minimize the number of devices that may encounter an unexpected update issue.</span></span> 

<span data-ttu-id="a4471-131">Saiba mais sobre o serviço de implantação:</span><span class="sxs-lookup"><span data-stu-id="a4471-131">Learn more about the deployment service:</span></span>
* [<span data-ttu-id="a4471-132">Atualizações de software</span><span class="sxs-lookup"><span data-stu-id="a4471-132">Software updates</span></span>](windowsupdates-software-updates.md)
* [<span data-ttu-id="a4471-133">Implantações</span><span class="sxs-lookup"><span data-stu-id="a4471-133">Deployments</span></span>](windowsupdates-deployments.md)
* [<span data-ttu-id="a4471-134">Agendar uma implantação</span><span class="sxs-lookup"><span data-stu-id="a4471-134">Schedule a deployment</span></span>](windowsupdates-schedule-deployment.md)

## <a name="immediately-deploy-an-update-when-critical-needs-arise"></a><span data-ttu-id="a4471-135">Implantar imediatamente uma atualização quando surgirem necessidades críticas</span><span class="sxs-lookup"><span data-stu-id="a4471-135">Immediately deploy an update when critical needs arise</span></span>

<span data-ttu-id="a4471-136">No caso de um problema crítico de segurança, você pode usar o serviço de implantação para ignorar uma política de atualização padrão e acelerar a implantação de uma atualização de segurança.</span><span class="sxs-lookup"><span data-stu-id="a4471-136">In the case of a critical security issue, you can use the deployment service to bypass a standard update policy and expedite deployment of a security update.</span></span>

<span data-ttu-id="a4471-137">Para saber mais, confira [Implantar uma atualização de segurança acelerada.](windowsupdates-deploy-expedited-update.md)</span><span class="sxs-lookup"><span data-stu-id="a4471-137">To learn more, see [Deploy an expedited security update](windowsupdates-deploy-expedited-update.md).</span></span>

## <a name="protect-devices-by-default"></a><span data-ttu-id="a4471-138">Proteger dispositivos por padrão</span><span class="sxs-lookup"><span data-stu-id="a4471-138">Protect devices by default</span></span>

<span data-ttu-id="a4471-139">Aproveite o benefício das [proteções](https://docs.microsoft.com/windows/deployment/update/safeguard-holds) de proteção que impedem que dispositivos com um problema de qualidade ou compatibilidade instalem uma atualização, resultando em falha ou reação de outra forma.</span><span class="sxs-lookup"><span data-stu-id="a4471-139">Enjoy the benefit of [safeguard holds](https://docs.microsoft.com/windows/deployment/update/safeguard-holds) which prevent devices with a quality or compatibility issue from installing an update, resulting in failure or rollback otherwise.</span></span>

<span data-ttu-id="a4471-140">Além disso, você pode configurar regras de monitoramento exclusivas da sua organização.</span><span class="sxs-lookup"><span data-stu-id="a4471-140">Additionally, you can configure monitoring rules that are unique to your organization.</span></span> <span data-ttu-id="a4471-141">Essas regras podem enviar um alerta ou pausar uma implantação com base em sinais de dispositivo, como reações.</span><span class="sxs-lookup"><span data-stu-id="a4471-141">These rules can send an alert or pause a deployment based on device signals such as rollbacks.</span></span>

<span data-ttu-id="a4471-142">Para saber mais, confira [Gerenciar regras de monitoramento para uma implantação](windowsupdates-manage-monitoring-rules.md).</span><span class="sxs-lookup"><span data-stu-id="a4471-142">To learn more, see [Manage monitoring rules for a deployment](windowsupdates-manage-monitoring-rules.md).</span></span>

## <a name="api-reference"></a><span data-ttu-id="a4471-143">Referência da API</span><span class="sxs-lookup"><span data-stu-id="a4471-143">API reference</span></span>

<span data-ttu-id="a4471-144">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="a4471-144">Looking for the API reference for this service?</span></span>

<span data-ttu-id="a4471-145">Consulte [Windows API de atualizações no Microsoft Graph beta](/graph/api/resources/windowsupdates-updates?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="a4471-145">See [Windows updates API in Microsoft Graph beta](/graph/api/resources/windowsupdates-updates?view=graph-rest-beta&preserve-view=true).</span></span>
