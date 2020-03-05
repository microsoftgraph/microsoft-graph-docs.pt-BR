---
title: tipo de enumeração policySetStatus
description: A enumeração para especificar o status de Policyset.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7164603d4de894936e236a98c58a0ef538a90d2b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523968"
---
# <a name="policysetstatus-enum-type"></a><span data-ttu-id="87d2a-103">tipo de enumeração policySetStatus</span><span class="sxs-lookup"><span data-stu-id="87d2a-103">policySetStatus enum type</span></span>

<span data-ttu-id="87d2a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="87d2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87d2a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87d2a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87d2a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87d2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87d2a-107">A enumeração para especificar o status de Policyset.</span><span class="sxs-lookup"><span data-stu-id="87d2a-107">The enum to specify the status of PolicySet.</span></span>

## <a name="members"></a><span data-ttu-id="87d2a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="87d2a-108">Members</span></span>
|<span data-ttu-id="87d2a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="87d2a-109">Member</span></span>|<span data-ttu-id="87d2a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="87d2a-110">Value</span></span>|<span data-ttu-id="87d2a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="87d2a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87d2a-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="87d2a-112">unknown</span></span>|<span data-ttu-id="87d2a-113">,0</span><span class="sxs-lookup"><span data-stu-id="87d2a-113">0</span></span>|<span data-ttu-id="87d2a-114">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="87d2a-114">Default Value.</span></span>|
|<span data-ttu-id="87d2a-115">conclui</span><span class="sxs-lookup"><span data-stu-id="87d2a-115">validating</span></span>|<span data-ttu-id="87d2a-116">1 </span><span class="sxs-lookup"><span data-stu-id="87d2a-116">1</span></span>|<span data-ttu-id="87d2a-117">Todos os itens de Policyset agora estão sendo validados para as configurações correspondentes de cargas de trabalho.</span><span class="sxs-lookup"><span data-stu-id="87d2a-117">All PolicySet items are now validating for corresponding settings of workloads.</span></span>|
|<span data-ttu-id="87d2a-118">partialSuccess</span><span class="sxs-lookup"><span data-stu-id="87d2a-118">partialSuccess</span></span>|<span data-ttu-id="87d2a-119">2 </span><span class="sxs-lookup"><span data-stu-id="87d2a-119">2</span></span>|<span data-ttu-id="87d2a-120">Processo de post concluído para todos os itens de Policyset, mas há falhas.</span><span class="sxs-lookup"><span data-stu-id="87d2a-120">Post process complete for all PolicySet items but there are failures.</span></span>|
|<span data-ttu-id="87d2a-121">sucesso</span><span class="sxs-lookup"><span data-stu-id="87d2a-121">success</span></span>|<span data-ttu-id="87d2a-122">3 </span><span class="sxs-lookup"><span data-stu-id="87d2a-122">3</span></span>|<span data-ttu-id="87d2a-123">Todos os itens de Policyset são implantados.</span><span class="sxs-lookup"><span data-stu-id="87d2a-123">All PolicySet items are deployed.</span></span> <span data-ttu-id="87d2a-124">Não significa que toda a implantação tenha sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="87d2a-124">Doesn’t mean that all deployment succeeded.</span></span> |
|<span data-ttu-id="87d2a-125">erro</span><span class="sxs-lookup"><span data-stu-id="87d2a-125">error</span></span>|<span data-ttu-id="87d2a-126">4 </span><span class="sxs-lookup"><span data-stu-id="87d2a-126">4</span></span>|<span data-ttu-id="87d2a-127">Falha total no processamento de policyset.</span><span class="sxs-lookup"><span data-stu-id="87d2a-127">PolicySet processing completely failed.</span></span>|
|<span data-ttu-id="87d2a-128">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="87d2a-128">notAssigned</span></span>|<span data-ttu-id="87d2a-129">5 </span><span class="sxs-lookup"><span data-stu-id="87d2a-129">5</span></span>|<span data-ttu-id="87d2a-130">Policyset/PolicySetItem não é atribuído a nenhum grupo.</span><span class="sxs-lookup"><span data-stu-id="87d2a-130">PolicySet/PolicySetItem is not assigned to any group.</span></span>|



