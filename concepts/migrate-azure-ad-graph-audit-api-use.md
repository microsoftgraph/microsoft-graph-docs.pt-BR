---
title: Examinar o uso do aplicativo APIs do Azure AD Graph
description: Descreve como auditar AS APIs do Azure Active Directory (Azure AD) para migrar um aplicativo para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: e7e21f03cdfd8ce3d45f0201d15ec489c7322530
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760690"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a><span data-ttu-id="fa797-103">Examinar o uso do aplicativo APIs do Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="fa797-103">Examine Azure AD Graph APIs app usage</span></span>

<span data-ttu-id="fa797-104">Esta é a etapa 2 do [processo para migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)</span><span class="sxs-lookup"><span data-stu-id="fa797-104">This is step 2 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="fa797-105">Ao planejar sua migração para o Microsoft Graph, leve tempo para revisar seu aplicativo existente e para catalogar as APIs do Azure AD Graph que você está usando no momento.</span><span class="sxs-lookup"><span data-stu-id="fa797-105">While planning your migration to Microsoft Graph, take time to review your existing application and to catalog the Azure AD Graph APIs you're currently using.</span></span>

<span data-ttu-id="fa797-106">Compare sua lista com as diferenças conhecidas.</span><span class="sxs-lookup"><span data-stu-id="fa797-106">Compare your list to the known differences.</span></span>  <span data-ttu-id="fa797-107">Isso ajuda a identificar alterações específicas que você precisará fazer para migrar seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fa797-107">This helps identify specific changes you'll need to make to migrate your app.</span></span>  <span data-ttu-id="fa797-108">Elas incluem alterações simples facilmente resolvidas usando os recursos de pesquisa e substituição de um editor ou atualizações mais complicadas que podem exigir mais análise.</span><span class="sxs-lookup"><span data-stu-id="fa797-108">These include simple changes easily resolved using an editor's search-and-replace features or more complicated updates that might require more analysis.</span></span>

<span data-ttu-id="fa797-109">O Microsoft Graph dá suporte a muitos dos mesmos recursos e recursos do gráfico do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fa797-109">Microsoft Graph supports many of the same features and capabilities of Azure AD graph.</span></span>  <span data-ttu-id="fa797-110">Há algumas diferenças importantes:</span><span class="sxs-lookup"><span data-stu-id="fa797-110">There are a few key differences:</span></span>

- [<span data-ttu-id="fa797-111">Diferenças de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa797-111">Request differences</span></span>](migrate-azure-ad-graph-request-differences.md)
- [<span data-ttu-id="fa797-112">Diferenças de recursos</span><span class="sxs-lookup"><span data-stu-id="fa797-112">Feature differences</span></span>](migrate-azure-ad-graph-feature-differences.md)
- [<span data-ttu-id="fa797-113">Diferenças de tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="fa797-113">Resource type differences</span></span>](migrate-azure-ad-graph-resource-differences.md)
- [<span data-ttu-id="fa797-114">Diferenças de propriedades</span><span class="sxs-lookup"><span data-stu-id="fa797-114">Property differences</span></span>](migrate-azure-ad-graph-property-differences.md)
- [<span data-ttu-id="fa797-115">Diferenças de método</span><span class="sxs-lookup"><span data-stu-id="fa797-115">Method differences</span></span>](migrate-azure-ad-graph-method-differences.md)

<span data-ttu-id="fa797-116">Você também vai querer verificar as permissões necessárias para os recursos que seu aplicativo está usando.</span><span class="sxs-lookup"><span data-stu-id="fa797-116">You'll also want to verify the permissions required for the features your app is using.</span></span>  <span data-ttu-id="fa797-117">Em alguns casos, permissões mais granulares estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="fa797-117">In some cases, more granular permissions are available.</span></span>

<span data-ttu-id="fa797-118">Para saber mais, confira [permissões](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa797-118">To learn more, see [Permissions](permissions-reference.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="fa797-119">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="fa797-119">Next Steps</span></span>

- <span data-ttu-id="fa797-120">Saiba mais [sobre o registro de aplicativos, permissões](migrate-azure-ad-graph-app-registration.md) e diferenças de consentimento entre o Azure AD Graph e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fa797-120">Learn about [app registration, permissions and consent differences](migrate-azure-ad-graph-app-registration.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="fa797-121">Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.</span><span class="sxs-lookup"><span data-stu-id="fa797-121">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>

