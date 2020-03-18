---
title: tipo de enumeração policySetStatus
description: A enumeração para especificar o status de Policyset.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a470e6c13bfd20ada920bbe2b471bfa96379092
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775146"
---
# <a name="policysetstatus-enum-type"></a><span data-ttu-id="126e9-103">tipo de enumeração policySetStatus</span><span class="sxs-lookup"><span data-stu-id="126e9-103">policySetStatus enum type</span></span>

> <span data-ttu-id="126e9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="126e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="126e9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="126e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="126e9-106">A enumeração para especificar o status de Policyset.</span><span class="sxs-lookup"><span data-stu-id="126e9-106">The enum to specify the status of PolicySet.</span></span>

## <a name="members"></a><span data-ttu-id="126e9-107">Membros</span><span class="sxs-lookup"><span data-stu-id="126e9-107">Members</span></span>
|<span data-ttu-id="126e9-108">Membro</span><span class="sxs-lookup"><span data-stu-id="126e9-108">Member</span></span>|<span data-ttu-id="126e9-109">Valor</span><span class="sxs-lookup"><span data-stu-id="126e9-109">Value</span></span>|<span data-ttu-id="126e9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="126e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="126e9-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="126e9-111">unknown</span></span>|<span data-ttu-id="126e9-112">,0</span><span class="sxs-lookup"><span data-stu-id="126e9-112">0</span></span>|<span data-ttu-id="126e9-113">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="126e9-113">Default Value.</span></span>|
|<span data-ttu-id="126e9-114">conclui</span><span class="sxs-lookup"><span data-stu-id="126e9-114">validating</span></span>|<span data-ttu-id="126e9-115">1</span><span class="sxs-lookup"><span data-stu-id="126e9-115">1</span></span>|<span data-ttu-id="126e9-116">Todos os itens de Policyset agora estão sendo validados para as configurações correspondentes de cargas de trabalho.</span><span class="sxs-lookup"><span data-stu-id="126e9-116">All PolicySet items are now validating for corresponding settings of workloads.</span></span>|
|<span data-ttu-id="126e9-117">partialSuccess</span><span class="sxs-lookup"><span data-stu-id="126e9-117">partialSuccess</span></span>|<span data-ttu-id="126e9-118">duas</span><span class="sxs-lookup"><span data-stu-id="126e9-118">2</span></span>|<span data-ttu-id="126e9-119">Processo de post concluído para todos os itens de Policyset, mas há falhas.</span><span class="sxs-lookup"><span data-stu-id="126e9-119">Post process complete for all PolicySet items but there are failures.</span></span>|
|<span data-ttu-id="126e9-120">sucesso</span><span class="sxs-lookup"><span data-stu-id="126e9-120">success</span></span>|<span data-ttu-id="126e9-121">3D</span><span class="sxs-lookup"><span data-stu-id="126e9-121">3</span></span>|<span data-ttu-id="126e9-122">Todos os itens de Policyset são implantados.</span><span class="sxs-lookup"><span data-stu-id="126e9-122">All PolicySet items are deployed.</span></span> <span data-ttu-id="126e9-123">Não significa que toda a implantação tenha sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="126e9-123">Doesn’t mean that all deployment succeeded.</span></span> |
|<span data-ttu-id="126e9-124">erro</span><span class="sxs-lookup"><span data-stu-id="126e9-124">error</span></span>|<span data-ttu-id="126e9-125">4 </span><span class="sxs-lookup"><span data-stu-id="126e9-125">4</span></span>|<span data-ttu-id="126e9-126">Falha total no processamento de policyset.</span><span class="sxs-lookup"><span data-stu-id="126e9-126">PolicySet processing completely failed.</span></span>|
|<span data-ttu-id="126e9-127">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="126e9-127">notAssigned</span></span>|<span data-ttu-id="126e9-128">5 </span><span class="sxs-lookup"><span data-stu-id="126e9-128">5</span></span>|<span data-ttu-id="126e9-129">Policyset/PolicySetItem não é atribuído a nenhum grupo.</span><span class="sxs-lookup"><span data-stu-id="126e9-129">PolicySet/PolicySetItem is not assigned to any group.</span></span>|



