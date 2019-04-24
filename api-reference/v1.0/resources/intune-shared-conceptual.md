---
title: Recursos compartilhados no Microsoft Intune
description: Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.  A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.  Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: cfb3acbb3b736fcb96d22773301ca6e2e3e4403f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32452180"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="3dcc9-105">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3dcc9-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="3dcc9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3dcc9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="3dcc9-107">Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.</span><span class="sxs-lookup"><span data-stu-id="3dcc9-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="3dcc9-108">A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="3dcc9-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="3dcc9-109">Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="3dcc9-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="3dcc9-110">Os seguintes recursos de gráfico são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="3dcc9-110">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="3dcc9-111">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="3dcc9-111">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="3dcc9-112">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="3dcc9-112">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="3dcc9-113">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="3dcc9-113">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="3dcc9-114">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="3dcc9-114">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="3dcc9-115">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="3dcc9-115">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="3dcc9-116">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3dcc9-116">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="3dcc9-117">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="3dcc9-117">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="3dcc9-118">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="3dcc9-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="3dcc9-119">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="3dcc9-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="3dcc9-120">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="3dcc9-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="3dcc9-121">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="3dcc9-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="3dcc9-122">Report</span><span class="sxs-lookup"><span data-stu-id="3dcc9-122">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="3dcc9-123">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="3dcc9-123">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="3dcc9-124">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="3dcc9-124">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="3dcc9-125">URI</span><span class="sxs-lookup"><span data-stu-id="3dcc9-125">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="3dcc9-126">Usuário</span><span class="sxs-lookup"><span data-stu-id="3dcc9-126">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="3dcc9-127">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="3dcc9-127">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
