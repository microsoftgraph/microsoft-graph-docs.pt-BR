---
title: Recursos compartilhados no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que dão suporte a vários fluxos de trabalho para uma organização de locatário.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 6436f134ae9e95623b073f6e645f0737d45d540e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158307"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="b0773-103">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b0773-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="b0773-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b0773-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0773-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b0773-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0773-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b0773-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b0773-107">Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.</span><span class="sxs-lookup"><span data-stu-id="b0773-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="b0773-108">A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="b0773-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="b0773-109">Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="b0773-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="b0773-110">Os seguintes recursos de gráfico são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="b0773-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="b0773-111">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="b0773-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="b0773-112">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="b0773-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="b0773-113">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="b0773-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="b0773-114">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="b0773-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="b0773-115">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="b0773-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="b0773-116">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b0773-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="b0773-117">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b0773-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="b0773-118">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b0773-118">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="b0773-119">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="b0773-119">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="b0773-120">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b0773-120">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="b0773-121">Tipo de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b0773-121">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="b0773-122">Habilitação</span><span class="sxs-lookup"><span data-stu-id="b0773-122">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="b0773-123">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="b0773-123">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="b0773-124">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="b0773-124">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="b0773-125">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="b0773-125">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="b0773-126">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="b0773-126">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="b0773-127">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="b0773-127">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="b0773-128">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="b0773-128">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="b0773-129">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="b0773-129">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="b0773-130">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="b0773-130">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="b0773-131">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="b0773-131">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="b0773-132">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="b0773-132">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="b0773-133">Report</span><span class="sxs-lookup"><span data-stu-id="b0773-133">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="b0773-134">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="b0773-134">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="b0773-135">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="b0773-135">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="b0773-136">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="b0773-136">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="b0773-137">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="b0773-137">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="b0773-138">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="b0773-138">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="b0773-139">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="b0773-139">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="b0773-140">URI</span><span class="sxs-lookup"><span data-stu-id="b0773-140">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="b0773-141">Usuário</span><span class="sxs-lookup"><span data-stu-id="b0773-141">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="b0773-142">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="b0773-142">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="b0773-143">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="b0773-143">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="b0773-144">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="b0773-144">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
