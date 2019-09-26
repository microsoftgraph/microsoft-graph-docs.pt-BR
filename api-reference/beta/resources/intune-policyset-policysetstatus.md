---
title: tipo de enumeração policySetStatus
description: A enumeração para especificar o status de Policyset.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a41e4f3dc01bd04c915dc4c883bae640b3e7683
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199631"
---
# <a name="policysetstatus-enum-type"></a><span data-ttu-id="27c5d-103">tipo de enumeração policySetStatus</span><span class="sxs-lookup"><span data-stu-id="27c5d-103">policySetStatus enum type</span></span>

> <span data-ttu-id="27c5d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27c5d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27c5d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27c5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27c5d-106">A enumeração para especificar o status de Policyset.</span><span class="sxs-lookup"><span data-stu-id="27c5d-106">The enum to specify the status of PolicySet.</span></span>

## <a name="members"></a><span data-ttu-id="27c5d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="27c5d-107">Members</span></span>
|<span data-ttu-id="27c5d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="27c5d-108">Member</span></span>|<span data-ttu-id="27c5d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="27c5d-109">Value</span></span>|<span data-ttu-id="27c5d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="27c5d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27c5d-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="27c5d-111">unknown</span></span>|<span data-ttu-id="27c5d-112">,0</span><span class="sxs-lookup"><span data-stu-id="27c5d-112">0</span></span>|<span data-ttu-id="27c5d-113">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="27c5d-113">Default Value.</span></span>|
|<span data-ttu-id="27c5d-114">conclui</span><span class="sxs-lookup"><span data-stu-id="27c5d-114">validating</span></span>|<span data-ttu-id="27c5d-115">1</span><span class="sxs-lookup"><span data-stu-id="27c5d-115">1</span></span>|<span data-ttu-id="27c5d-116">Todos os itens de Policyset agora estão sendo validados para as configurações correspondentes de cargas de trabalho.</span><span class="sxs-lookup"><span data-stu-id="27c5d-116">All PolicySet items are now validating for corresponding settings of workloads.</span></span>|
|<span data-ttu-id="27c5d-117">partialSuccess</span><span class="sxs-lookup"><span data-stu-id="27c5d-117">partialSuccess</span></span>|<span data-ttu-id="27c5d-118">duas</span><span class="sxs-lookup"><span data-stu-id="27c5d-118">2</span></span>|<span data-ttu-id="27c5d-119">Processo de post concluído para todos os itens de Policyset, mas há falhas.</span><span class="sxs-lookup"><span data-stu-id="27c5d-119">Post process complete for all PolicySet items but there are failures.</span></span>|
|<span data-ttu-id="27c5d-120">sucesso</span><span class="sxs-lookup"><span data-stu-id="27c5d-120">success</span></span>|<span data-ttu-id="27c5d-121">3D</span><span class="sxs-lookup"><span data-stu-id="27c5d-121">3</span></span>|<span data-ttu-id="27c5d-122">Todos os itens de Policyset são implantados.</span><span class="sxs-lookup"><span data-stu-id="27c5d-122">All PolicySet items are deployed.</span></span> <span data-ttu-id="27c5d-123">Não significa que toda a implantação tenha sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="27c5d-123">Doesn’t mean that all deployment succeeded.</span></span> |
|<span data-ttu-id="27c5d-124">erro</span><span class="sxs-lookup"><span data-stu-id="27c5d-124">error</span></span>|<span data-ttu-id="27c5d-125">quatro</span><span class="sxs-lookup"><span data-stu-id="27c5d-125">4</span></span>|<span data-ttu-id="27c5d-126">Falha total no processamento de policyset.</span><span class="sxs-lookup"><span data-stu-id="27c5d-126">PolicySet processing completely failed.</span></span>|
|<span data-ttu-id="27c5d-127">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="27c5d-127">notAssigned</span></span>|<span data-ttu-id="27c5d-128">0,5</span><span class="sxs-lookup"><span data-stu-id="27c5d-128">5</span></span>|<span data-ttu-id="27c5d-129">Policyset/PolicySetItem não é atribuído a nenhum grupo.</span><span class="sxs-lookup"><span data-stu-id="27c5d-129">PolicySet/PolicySetItem is not assigned to any group.</span></span>|



