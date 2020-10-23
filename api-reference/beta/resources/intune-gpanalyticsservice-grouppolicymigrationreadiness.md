---
title: tipo de enumeração groupPolicyMigrationReadiness
description: Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d860844de50c58deace7f10821ca0b1a4591d00b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722820"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="c2b9d-103">tipo de enumeração groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="c2b9d-103">groupPolicyMigrationReadiness enum type</span></span>

<span data-ttu-id="c2b9d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2b9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2b9d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c2b9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2b9d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2b9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2b9d-107">Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.</span><span class="sxs-lookup"><span data-stu-id="c2b9d-107">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="c2b9d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c2b9d-108">Members</span></span>
|<span data-ttu-id="c2b9d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c2b9d-109">Member</span></span>|<span data-ttu-id="c2b9d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c2b9d-110">Value</span></span>|<span data-ttu-id="c2b9d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2b9d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2b9d-112">none</span><span class="sxs-lookup"><span data-stu-id="c2b9d-112">none</span></span>|<span data-ttu-id="c2b9d-113">1</span><span class="sxs-lookup"><span data-stu-id="c2b9d-113">1</span></span>|<span data-ttu-id="c2b9d-114">Nenhuma cobertura do Intune</span><span class="sxs-lookup"><span data-stu-id="c2b9d-114">No Intune coverage</span></span>|
|<span data-ttu-id="c2b9d-115">parcial</span><span class="sxs-lookup"><span data-stu-id="c2b9d-115">partial</span></span>|<span data-ttu-id="c2b9d-116">duas</span><span class="sxs-lookup"><span data-stu-id="c2b9d-116">2</span></span>|<span data-ttu-id="c2b9d-117">Cobertura do Intune parcial</span><span class="sxs-lookup"><span data-stu-id="c2b9d-117">Partial Intune coverage</span></span>|
|<span data-ttu-id="c2b9d-118">complete</span><span class="sxs-lookup"><span data-stu-id="c2b9d-118">complete</span></span>|<span data-ttu-id="c2b9d-119">3D</span><span class="sxs-lookup"><span data-stu-id="c2b9d-119">3</span></span>|<span data-ttu-id="c2b9d-120">Cobertura completa do Intune</span><span class="sxs-lookup"><span data-stu-id="c2b9d-120">Complete Intune coverage</span></span>|
|<span data-ttu-id="c2b9d-121">erro</span><span class="sxs-lookup"><span data-stu-id="c2b9d-121">error</span></span>|<span data-ttu-id="c2b9d-122">4 </span><span class="sxs-lookup"><span data-stu-id="c2b9d-122">4</span></span>|<span data-ttu-id="c2b9d-123">Erro ao analisar a cobertura</span><span class="sxs-lookup"><span data-stu-id="c2b9d-123">Error when analyzing coverage</span></span>|
|<span data-ttu-id="c2b9d-124">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="c2b9d-124">notApplicable</span></span>|<span data-ttu-id="c2b9d-125">5 </span><span class="sxs-lookup"><span data-stu-id="c2b9d-125">5</span></span>|<span data-ttu-id="c2b9d-126">Nenhuma configuração de política de grupo no GPO</span><span class="sxs-lookup"><span data-stu-id="c2b9d-126">No Group Policy settings in GPO</span></span>|





