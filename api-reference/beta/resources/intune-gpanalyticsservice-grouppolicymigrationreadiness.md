---
title: tipo de enumeração groupPolicyMigrationReadiness
description: Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: efd579adb3c3408eda9b87ffb7f48e98c836065f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783169"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="3e865-103">tipo de enumeração groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="3e865-103">groupPolicyMigrationReadiness enum type</span></span>

> <span data-ttu-id="3e865-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3e865-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e865-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e865-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e865-106">Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.</span><span class="sxs-lookup"><span data-stu-id="3e865-106">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="3e865-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3e865-107">Members</span></span>
|<span data-ttu-id="3e865-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3e865-108">Member</span></span>|<span data-ttu-id="3e865-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3e865-109">Value</span></span>|<span data-ttu-id="3e865-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e865-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e865-111">none</span><span class="sxs-lookup"><span data-stu-id="3e865-111">none</span></span>|<span data-ttu-id="3e865-112">1</span><span class="sxs-lookup"><span data-stu-id="3e865-112">1</span></span>|<span data-ttu-id="3e865-113">Nenhuma cobertura do Intune</span><span class="sxs-lookup"><span data-stu-id="3e865-113">No Intune coverage</span></span>|
|<span data-ttu-id="3e865-114">parcial</span><span class="sxs-lookup"><span data-stu-id="3e865-114">partial</span></span>|<span data-ttu-id="3e865-115">duas</span><span class="sxs-lookup"><span data-stu-id="3e865-115">2</span></span>|<span data-ttu-id="3e865-116">Cobertura do Intune parcial</span><span class="sxs-lookup"><span data-stu-id="3e865-116">Partial Intune coverage</span></span>|
|<span data-ttu-id="3e865-117">complete</span><span class="sxs-lookup"><span data-stu-id="3e865-117">complete</span></span>|<span data-ttu-id="3e865-118">3D</span><span class="sxs-lookup"><span data-stu-id="3e865-118">3</span></span>|<span data-ttu-id="3e865-119">Cobertura completa do Intune</span><span class="sxs-lookup"><span data-stu-id="3e865-119">Complete Intune coverage</span></span>|
|<span data-ttu-id="3e865-120">erro</span><span class="sxs-lookup"><span data-stu-id="3e865-120">error</span></span>|<span data-ttu-id="3e865-121">4 </span><span class="sxs-lookup"><span data-stu-id="3e865-121">4</span></span>|<span data-ttu-id="3e865-122">Erro ao analisar a cobertura</span><span class="sxs-lookup"><span data-stu-id="3e865-122">Error when analyzing coverage</span></span>|
|<span data-ttu-id="3e865-123">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="3e865-123">notApplicable</span></span>|<span data-ttu-id="3e865-124">5 </span><span class="sxs-lookup"><span data-stu-id="3e865-124">5</span></span>|<span data-ttu-id="3e865-125">Nenhuma configuração de política de grupo no GPO</span><span class="sxs-lookup"><span data-stu-id="3e865-125">No Group Policy settings in GPO</span></span>|



