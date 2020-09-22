---
title: tipo de enumeração groupPolicyMigrationReadiness
description: Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 15e7d0a626934f8f6d17aebf6eff9aff8c537dbd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031225"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="38423-103">tipo de enumeração groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="38423-103">groupPolicyMigrationReadiness enum type</span></span>

<span data-ttu-id="38423-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38423-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38423-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="38423-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38423-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38423-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38423-107">Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.</span><span class="sxs-lookup"><span data-stu-id="38423-107">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="38423-108">Membros</span><span class="sxs-lookup"><span data-stu-id="38423-108">Members</span></span>
|<span data-ttu-id="38423-109">Membro</span><span class="sxs-lookup"><span data-stu-id="38423-109">Member</span></span>|<span data-ttu-id="38423-110">Valor</span><span class="sxs-lookup"><span data-stu-id="38423-110">Value</span></span>|<span data-ttu-id="38423-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="38423-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38423-112">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="38423-112">none</span></span>|<span data-ttu-id="38423-113">1 </span><span class="sxs-lookup"><span data-stu-id="38423-113">1</span></span>|<span data-ttu-id="38423-114">Nenhuma cobertura do Intune</span><span class="sxs-lookup"><span data-stu-id="38423-114">No Intune coverage</span></span>|
|<span data-ttu-id="38423-115">parcial</span><span class="sxs-lookup"><span data-stu-id="38423-115">partial</span></span>|<span data-ttu-id="38423-116">2 </span><span class="sxs-lookup"><span data-stu-id="38423-116">2</span></span>|<span data-ttu-id="38423-117">Cobertura do Intune parcial</span><span class="sxs-lookup"><span data-stu-id="38423-117">Partial Intune coverage</span></span>|
|<span data-ttu-id="38423-118">complete</span><span class="sxs-lookup"><span data-stu-id="38423-118">complete</span></span>|<span data-ttu-id="38423-119">3 </span><span class="sxs-lookup"><span data-stu-id="38423-119">3</span></span>|<span data-ttu-id="38423-120">Cobertura completa do Intune</span><span class="sxs-lookup"><span data-stu-id="38423-120">Complete Intune coverage</span></span>|
|<span data-ttu-id="38423-121">erro</span><span class="sxs-lookup"><span data-stu-id="38423-121">error</span></span>|<span data-ttu-id="38423-122">4 </span><span class="sxs-lookup"><span data-stu-id="38423-122">4</span></span>|<span data-ttu-id="38423-123">Erro ao analisar a cobertura</span><span class="sxs-lookup"><span data-stu-id="38423-123">Error when analyzing coverage</span></span>|
|<span data-ttu-id="38423-124">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="38423-124">notApplicable</span></span>|<span data-ttu-id="38423-125">5 </span><span class="sxs-lookup"><span data-stu-id="38423-125">5</span></span>|<span data-ttu-id="38423-126">Nenhuma configuração de política de grupo no GPO</span><span class="sxs-lookup"><span data-stu-id="38423-126">No Group Policy settings in GPO</span></span>|






