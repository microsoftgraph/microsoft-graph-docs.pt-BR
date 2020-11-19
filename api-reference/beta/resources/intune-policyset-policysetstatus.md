---
title: tipo de enumeração policySetStatus
description: A enumeração para especificar o status de Policyset.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ffadd40f791971fa0225a893959e4224c51070f5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287904"
---
# <a name="policysetstatus-enum-type"></a><span data-ttu-id="11ae1-103">tipo de enumeração policySetStatus</span><span class="sxs-lookup"><span data-stu-id="11ae1-103">policySetStatus enum type</span></span>

<span data-ttu-id="11ae1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11ae1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11ae1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11ae1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11ae1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11ae1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11ae1-107">A enumeração para especificar o status de Policyset.</span><span class="sxs-lookup"><span data-stu-id="11ae1-107">The enum to specify the status of PolicySet.</span></span>

## <a name="members"></a><span data-ttu-id="11ae1-108">Membros</span><span class="sxs-lookup"><span data-stu-id="11ae1-108">Members</span></span>
|<span data-ttu-id="11ae1-109">Membro</span><span class="sxs-lookup"><span data-stu-id="11ae1-109">Member</span></span>|<span data-ttu-id="11ae1-110">Valor</span><span class="sxs-lookup"><span data-stu-id="11ae1-110">Value</span></span>|<span data-ttu-id="11ae1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="11ae1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11ae1-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="11ae1-112">unknown</span></span>|<span data-ttu-id="11ae1-113">,0</span><span class="sxs-lookup"><span data-stu-id="11ae1-113">0</span></span>|<span data-ttu-id="11ae1-114">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="11ae1-114">Default Value.</span></span>|
|<span data-ttu-id="11ae1-115">conclui</span><span class="sxs-lookup"><span data-stu-id="11ae1-115">validating</span></span>|<span data-ttu-id="11ae1-116">1</span><span class="sxs-lookup"><span data-stu-id="11ae1-116">1</span></span>|<span data-ttu-id="11ae1-117">Todos os itens de Policyset agora estão sendo validados para as configurações correspondentes de cargas de trabalho.</span><span class="sxs-lookup"><span data-stu-id="11ae1-117">All PolicySet items are now validating for corresponding settings of workloads.</span></span>|
|<span data-ttu-id="11ae1-118">partialSuccess</span><span class="sxs-lookup"><span data-stu-id="11ae1-118">partialSuccess</span></span>|<span data-ttu-id="11ae1-119">duas</span><span class="sxs-lookup"><span data-stu-id="11ae1-119">2</span></span>|<span data-ttu-id="11ae1-120">Processo de post concluído para todos os itens de Policyset, mas há falhas.</span><span class="sxs-lookup"><span data-stu-id="11ae1-120">Post process complete for all PolicySet items but there are failures.</span></span>|
|<span data-ttu-id="11ae1-121">sucesso</span><span class="sxs-lookup"><span data-stu-id="11ae1-121">success</span></span>|<span data-ttu-id="11ae1-122">3D</span><span class="sxs-lookup"><span data-stu-id="11ae1-122">3</span></span>|<span data-ttu-id="11ae1-123">Todos os itens de Policyset são implantados.</span><span class="sxs-lookup"><span data-stu-id="11ae1-123">All PolicySet items are deployed.</span></span> <span data-ttu-id="11ae1-124">Não significa que toda a implantação tenha sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="11ae1-124">Doesn’t mean that all deployment succeeded.</span></span> |
|<span data-ttu-id="11ae1-125">erro</span><span class="sxs-lookup"><span data-stu-id="11ae1-125">error</span></span>|<span data-ttu-id="11ae1-126">4 </span><span class="sxs-lookup"><span data-stu-id="11ae1-126">4</span></span>|<span data-ttu-id="11ae1-127">Falha total no processamento de policyset.</span><span class="sxs-lookup"><span data-stu-id="11ae1-127">PolicySet processing completely failed.</span></span>|
|<span data-ttu-id="11ae1-128">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="11ae1-128">notAssigned</span></span>|<span data-ttu-id="11ae1-129">5 </span><span class="sxs-lookup"><span data-stu-id="11ae1-129">5</span></span>|<span data-ttu-id="11ae1-130">Policyset/PolicySetItem não é atribuído a nenhum grupo.</span><span class="sxs-lookup"><span data-stu-id="11ae1-130">PolicySet/PolicySetItem is not assigned to any group.</span></span>|




