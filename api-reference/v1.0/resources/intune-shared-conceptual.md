---
title: Recursos compartilhados no Microsoft Intune
description: Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.  A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.  Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: cc5cbf0f96d3c9199ecd9b622d9724ec10dd472e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037651"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="b1335-105">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b1335-105">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="b1335-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1335-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1335-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b1335-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b1335-108">Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.</span><span class="sxs-lookup"><span data-stu-id="b1335-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="b1335-109">A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="b1335-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="b1335-110">Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="b1335-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="b1335-111">Os seguintes recursos de gráfico são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="b1335-111">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="b1335-112">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="b1335-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="b1335-113">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="b1335-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="b1335-114">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="b1335-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="b1335-115">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="b1335-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="b1335-116">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b1335-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="b1335-117">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b1335-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="b1335-118">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="b1335-118">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="b1335-119">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="b1335-119">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="b1335-120">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="b1335-120">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="b1335-121">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="b1335-121">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="b1335-122">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="b1335-122">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="b1335-123">Relatório</span><span class="sxs-lookup"><span data-stu-id="b1335-123">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="b1335-124">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="b1335-124">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="b1335-125">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="b1335-125">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="b1335-126">URI</span><span class="sxs-lookup"><span data-stu-id="b1335-126">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="b1335-127">Usuário</span><span class="sxs-lookup"><span data-stu-id="b1335-127">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="b1335-128">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="b1335-128">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)






