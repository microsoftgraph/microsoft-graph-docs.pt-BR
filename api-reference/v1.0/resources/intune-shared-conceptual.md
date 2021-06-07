---
title: Recursos compartilhados em Microsoft Intune
description: Esses pontos de extremidade são usados em várias API do Microsoft Graph para fluxos de trabalho do Intune.  A intenção, a finalidade e as permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.  Além disso, determinados métodos, propriedades e ações são suportados apenas para fluxos de trabalho específicos.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: cc5cbf0f96d3c9199ecd9b622d9724ec10dd472e
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732231"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="b02f9-105">Recursos compartilhados em Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b02f9-105">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="b02f9-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b02f9-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b02f9-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b02f9-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b02f9-108">Esses pontos de extremidade são usados em várias API do Microsoft Graph para fluxos de trabalho do Intune.</span><span class="sxs-lookup"><span data-stu-id="b02f9-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="b02f9-109">A intenção, a finalidade e as permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="b02f9-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="b02f9-110">Além disso, determinados métodos, propriedades e ações são suportados apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="b02f9-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="b02f9-111">Os seguintes Graph são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="b02f9-111">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="b02f9-112">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="b02f9-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="b02f9-113">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="b02f9-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="b02f9-114">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="b02f9-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="b02f9-115">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="b02f9-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="b02f9-116">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b02f9-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="b02f9-117">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b02f9-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="b02f9-118">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="b02f9-118">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="b02f9-119">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="b02f9-119">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="b02f9-120">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="b02f9-120">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="b02f9-121">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="b02f9-121">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="b02f9-122">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="b02f9-122">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="b02f9-123">Relatório</span><span class="sxs-lookup"><span data-stu-id="b02f9-123">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="b02f9-124">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="b02f9-124">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="b02f9-125">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="b02f9-125">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="b02f9-126">URI</span><span class="sxs-lookup"><span data-stu-id="b02f9-126">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="b02f9-127">Usuário</span><span class="sxs-lookup"><span data-stu-id="b02f9-127">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="b02f9-128">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="b02f9-128">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)






