---
title: Examinar o uso do aplicativo APIs do Azure AD Graph
description: Descreve como auditar as APIs do Azure Active Directory (Azure AD) para migrar um aplicativo para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14cc61039d97fa43f64599310cf86cce6c348fb2
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645244"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a><span data-ttu-id="a3642-103">Examinar o uso do aplicativo APIs do Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="a3642-103">Examine Azure AD Graph APIs app usage</span></span>

<span data-ttu-id="a3642-104">Esta é a etapa 2 do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="a3642-104">This is step 2 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="a3642-105">Ao planejar sua migração para o Microsoft Graph, Reserve um tempo para revisar seu aplicativo existente e catalogar as APIs do Azure AD Graph que você está usando no momento.</span><span class="sxs-lookup"><span data-stu-id="a3642-105">While planning your migration to Microsoft Graph, take time to review your existing application and to catalog the Azure AD Graph APIs you're currently using.</span></span>

<span data-ttu-id="a3642-106">Compare sua lista com as diferenças conhecidas.</span><span class="sxs-lookup"><span data-stu-id="a3642-106">Compare your list to the known differences.</span></span>  <span data-ttu-id="a3642-107">Isso ajuda a identificar alterações específicas que você precisará fazer para migrar seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a3642-107">This helps identify specific changes you'll need to make to migrate your app.</span></span>  <span data-ttu-id="a3642-108">Eles incluem alterações simples facilmente resolvidas usando os recursos de pesquisa e substituição de um editor ou atualizações mais complicadas que podem exigir mais análise.</span><span class="sxs-lookup"><span data-stu-id="a3642-108">These include simple changes easily resolved using an editor's search-and-replace features or more complicated updates that might require more analysis.</span></span>

<span data-ttu-id="a3642-109">O Microsoft Graph oferece suporte a muitos dos mesmos recursos e funcionalidades do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="a3642-109">Microsoft Graph supports many of the same features and capabilities of Azure AD graph.</span></span>  <span data-ttu-id="a3642-110">Há algumas diferenças importantes:</span><span class="sxs-lookup"><span data-stu-id="a3642-110">There are a few key differences:</span></span>

- [<span data-ttu-id="a3642-111">Solicitar diferenças</span><span class="sxs-lookup"><span data-stu-id="a3642-111">Request differences</span></span>](migrate-azure-ad-graph-request-differences.md)
- [<span data-ttu-id="a3642-112">Diferenças de recursos</span><span class="sxs-lookup"><span data-stu-id="a3642-112">Feature differences</span></span>](migrate-azure-ad-graph-feature-differences.md)
- [<span data-ttu-id="a3642-113">Diferenças de tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="a3642-113">Resource type differences</span></span>](migrate-azure-ad-graph-resource-differences.md)
- [<span data-ttu-id="a3642-114">Diferenças de propriedade</span><span class="sxs-lookup"><span data-stu-id="a3642-114">Property differences</span></span>](migrate-azure-ad-graph-property-differences.md)
- [<span data-ttu-id="a3642-115">Diferenças de método</span><span class="sxs-lookup"><span data-stu-id="a3642-115">Method differences</span></span>](migrate-azure-ad-graph-method-differences.md)

<span data-ttu-id="a3642-116">Você também deve verificar as permissões necessárias para os recursos que seu aplicativo está usando.</span><span class="sxs-lookup"><span data-stu-id="a3642-116">You'll also want to verify the permissions required for the features your app is using.</span></span>  <span data-ttu-id="a3642-117">Em alguns casos, as permissões mais granulares estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="a3642-117">In some cases, more granular permissions are available.</span></span>

<span data-ttu-id="a3642-118">Para saber mais, confira [permissões](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a3642-118">To learn more, see [Permissions](permissions-reference.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="a3642-119">Próximos passos</span><span class="sxs-lookup"><span data-stu-id="a3642-119">Next Steps</span></span>

- <span data-ttu-id="a3642-120">Saiba mais sobre [as diferenças de registro de aplicativo, permissões e consentimento](migrate-azure-ad-graph-app-registration.md) entre o Azure ad Graph e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a3642-120">Learn about [app registration, permissions and consent differences](migrate-azure-ad-graph-app-registration.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="a3642-121">Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="a3642-121">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="a3642-122">Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a3642-122">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
