---
title: tipo de enumeração groupPolicyMigrationReadiness
description: Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d05a88dd1e9aacb36968b99c2ec797c8ac3bf01f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458473"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="e8f24-103">tipo de enumeração groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="e8f24-103">groupPolicyMigrationReadiness enum type</span></span>

<span data-ttu-id="e8f24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8f24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8f24-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8f24-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8f24-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8f24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8f24-107">Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.</span><span class="sxs-lookup"><span data-stu-id="e8f24-107">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="e8f24-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e8f24-108">Members</span></span>
|<span data-ttu-id="e8f24-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e8f24-109">Member</span></span>|<span data-ttu-id="e8f24-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e8f24-110">Value</span></span>|<span data-ttu-id="e8f24-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8f24-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8f24-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="e8f24-112">none</span></span>|<span data-ttu-id="e8f24-113">1</span><span class="sxs-lookup"><span data-stu-id="e8f24-113">1</span></span>|<span data-ttu-id="e8f24-114">Nenhuma cobertura do Intune</span><span class="sxs-lookup"><span data-stu-id="e8f24-114">No Intune coverage</span></span>|
|<span data-ttu-id="e8f24-115">parcial</span><span class="sxs-lookup"><span data-stu-id="e8f24-115">partial</span></span>|<span data-ttu-id="e8f24-116">duas</span><span class="sxs-lookup"><span data-stu-id="e8f24-116">2</span></span>|<span data-ttu-id="e8f24-117">Cobertura do Intune parcial</span><span class="sxs-lookup"><span data-stu-id="e8f24-117">Partial Intune coverage</span></span>|
|<span data-ttu-id="e8f24-118">complete</span><span class="sxs-lookup"><span data-stu-id="e8f24-118">complete</span></span>|<span data-ttu-id="e8f24-119">3D</span><span class="sxs-lookup"><span data-stu-id="e8f24-119">3</span></span>|<span data-ttu-id="e8f24-120">Cobertura completa do Intune</span><span class="sxs-lookup"><span data-stu-id="e8f24-120">Complete Intune coverage</span></span>|
|<span data-ttu-id="e8f24-121">erro</span><span class="sxs-lookup"><span data-stu-id="e8f24-121">error</span></span>|<span data-ttu-id="e8f24-122">4 </span><span class="sxs-lookup"><span data-stu-id="e8f24-122">4</span></span>|<span data-ttu-id="e8f24-123">Erro ao analisar a cobertura</span><span class="sxs-lookup"><span data-stu-id="e8f24-123">Error when analyzing coverage</span></span>|
|<span data-ttu-id="e8f24-124">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="e8f24-124">notApplicable</span></span>|<span data-ttu-id="e8f24-125">5 </span><span class="sxs-lookup"><span data-stu-id="e8f24-125">5</span></span>|<span data-ttu-id="e8f24-126">Nenhuma configuração de política de grupo no GPO</span><span class="sxs-lookup"><span data-stu-id="e8f24-126">No Group Policy settings in GPO</span></span>|



