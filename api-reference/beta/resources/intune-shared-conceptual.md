---
title: Recursos compartilhados no Microsoft Intune
description: Esses pontos de extremidade são usados em vários API do Microsoft Graph Intune fluxos de trabalho.  A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.  Além disso, determinados métodos, propriedades e ações são suportadas somente para fluxos de trabalho específicos.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 6180868d4aec195afcc037146f475e56a91aa669
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952556"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="93ff3-105">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="93ff3-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="93ff3-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="93ff3-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93ff3-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="93ff3-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93ff3-108">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="93ff3-108">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="93ff3-109">Esses pontos de extremidade são usados em vários API do Microsoft Graph Intune fluxos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="93ff3-109">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="93ff3-110">A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="93ff3-110">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="93ff3-111">Além disso, determinados métodos, propriedades e ações são suportadas somente para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="93ff3-111">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="93ff3-112">Os recursos de gráfico a seguir são compartilhados entre o Intune fluxos de trabalho:</span><span class="sxs-lookup"><span data-stu-id="93ff3-112">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="93ff3-113">Estado de ação</span><span class="sxs-lookup"><span data-stu-id="93ff3-113">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="93ff3-114">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="93ff3-114">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="93ff3-115">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="93ff3-115">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="93ff3-116">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="93ff3-116">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="93ff3-117">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="93ff3-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="93ff3-118">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="93ff3-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="93ff3-119">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="93ff3-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="93ff3-120">Tipo de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="93ff3-120">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="93ff3-121">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="93ff3-121">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="93ff3-122">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="93ff3-122">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="93ff3-123">Tipo de dispositivo</span><span class="sxs-lookup"><span data-stu-id="93ff3-123">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="93ff3-124">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="93ff3-124">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="93ff3-125">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="93ff3-125">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="93ff3-126">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="93ff3-126">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="93ff3-127">Instalar a intenção</span><span class="sxs-lookup"><span data-stu-id="93ff3-127">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="93ff3-128">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="93ff3-128">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="93ff3-129">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="93ff3-129">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="93ff3-130">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="93ff3-130">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="93ff3-131">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="93ff3-131">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="93ff3-132">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="93ff3-132">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="93ff3-133">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="93ff3-133">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="93ff3-134">Report</span><span class="sxs-lookup"><span data-stu-id="93ff3-134">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="93ff3-135">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="93ff3-135">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="93ff3-136">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="93ff3-136">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="93ff3-137">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="93ff3-137">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="93ff3-138">Executar como do tipo de conta</span><span class="sxs-lookup"><span data-stu-id="93ff3-138">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="93ff3-139">Executada no estado</span><span class="sxs-lookup"><span data-stu-id="93ff3-139">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="93ff3-140">Salva as opções de geração de estado da interface do usuário</span><span class="sxs-lookup"><span data-stu-id="93ff3-140">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="93ff3-141">URI</span><span class="sxs-lookup"><span data-stu-id="93ff3-141">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="93ff3-142">Usuário</span><span class="sxs-lookup"><span data-stu-id="93ff3-142">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="93ff3-143">Tipo de conta de token de VPP</span><span class="sxs-lookup"><span data-stu-id="93ff3-143">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="93ff3-144">Motivo da falha VPP ação token</span><span class="sxs-lookup"><span data-stu-id="93ff3-144">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="93ff3-145">Configuração de ingresso de domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="93ff3-145">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
