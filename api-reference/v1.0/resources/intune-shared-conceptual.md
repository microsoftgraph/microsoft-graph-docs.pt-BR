---
title: Recursos compartilhados em Microsoft Intune
description: Esses pontos de extremidade são usados em várias API do Microsoft Graph para fluxos de trabalho do Intune.  A intenção, a finalidade e as permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.  Além disso, determinados métodos, propriedades e ações são suportados apenas para fluxos de trabalho específicos.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 0af56b1ec3014fdee14dc4b70d3c14208321581a
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108884"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="ec16f-105">Recursos compartilhados em Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ec16f-105">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="ec16f-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec16f-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec16f-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ec16f-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="ec16f-108">Esses pontos de extremidade são usados em várias API do Microsoft Graph para fluxos de trabalho do Intune.</span><span class="sxs-lookup"><span data-stu-id="ec16f-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="ec16f-109">A intenção, a finalidade e as permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="ec16f-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="ec16f-110">Além disso, determinados métodos, propriedades e ações são suportados apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="ec16f-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="ec16f-111">Os seguintes Graph são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="ec16f-111">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="ec16f-112">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="ec16f-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="ec16f-113">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="ec16f-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="ec16f-114">Android enterprise sempre no tipo de pacote VPN</span><span class="sxs-lookup"><span data-stu-id="ec16f-114">Android enterprise always on VPN package type</span></span>](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [<span data-ttu-id="ec16f-115">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="ec16f-115">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="ec16f-116">Destino da atribuição da coleção configuration manager</span><span class="sxs-lookup"><span data-stu-id="ec16f-116">Configuration manager collection assignment target</span></span>](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [<span data-ttu-id="ec16f-117">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec16f-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="ec16f-118">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="ec16f-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="ec16f-119">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="ec16f-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="ec16f-120">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="ec16f-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="ec16f-121">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="ec16f-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="ec16f-122">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="ec16f-122">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="ec16f-123">URI</span><span class="sxs-lookup"><span data-stu-id="ec16f-123">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="ec16f-124">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="ec16f-124">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)