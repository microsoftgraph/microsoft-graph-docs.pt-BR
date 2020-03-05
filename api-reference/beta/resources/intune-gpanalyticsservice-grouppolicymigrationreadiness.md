---
title: tipo de enumeração groupPolicyMigrationReadiness
description: Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e6b2ec4f8363f6ad68cd34a77287502eaadf2d52
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524480"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="98405-103">tipo de enumeração groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="98405-103">groupPolicyMigrationReadiness enum type</span></span>

<span data-ttu-id="98405-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="98405-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98405-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="98405-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98405-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98405-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98405-107">Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.</span><span class="sxs-lookup"><span data-stu-id="98405-107">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="98405-108">Membros</span><span class="sxs-lookup"><span data-stu-id="98405-108">Members</span></span>
|<span data-ttu-id="98405-109">Membro</span><span class="sxs-lookup"><span data-stu-id="98405-109">Member</span></span>|<span data-ttu-id="98405-110">Valor</span><span class="sxs-lookup"><span data-stu-id="98405-110">Value</span></span>|<span data-ttu-id="98405-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="98405-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98405-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="98405-112">none</span></span>|<span data-ttu-id="98405-113">1 </span><span class="sxs-lookup"><span data-stu-id="98405-113">1</span></span>|<span data-ttu-id="98405-114">Nenhuma cobertura do Intune</span><span class="sxs-lookup"><span data-stu-id="98405-114">No Intune coverage</span></span>|
|<span data-ttu-id="98405-115">parcial</span><span class="sxs-lookup"><span data-stu-id="98405-115">partial</span></span>|<span data-ttu-id="98405-116">2 </span><span class="sxs-lookup"><span data-stu-id="98405-116">2</span></span>|<span data-ttu-id="98405-117">Cobertura do Intune parcial</span><span class="sxs-lookup"><span data-stu-id="98405-117">Partial Intune coverage</span></span>|
|<span data-ttu-id="98405-118">complete</span><span class="sxs-lookup"><span data-stu-id="98405-118">complete</span></span>|<span data-ttu-id="98405-119">3 </span><span class="sxs-lookup"><span data-stu-id="98405-119">3</span></span>|<span data-ttu-id="98405-120">Cobertura completa do Intune</span><span class="sxs-lookup"><span data-stu-id="98405-120">Complete Intune coverage</span></span>|
|<span data-ttu-id="98405-121">erro</span><span class="sxs-lookup"><span data-stu-id="98405-121">error</span></span>|<span data-ttu-id="98405-122">4 </span><span class="sxs-lookup"><span data-stu-id="98405-122">4</span></span>|<span data-ttu-id="98405-123">Erro ao analisar a cobertura</span><span class="sxs-lookup"><span data-stu-id="98405-123">Error when analyzing coverage</span></span>|
|<span data-ttu-id="98405-124">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="98405-124">notApplicable</span></span>|<span data-ttu-id="98405-125">5 </span><span class="sxs-lookup"><span data-stu-id="98405-125">5</span></span>|<span data-ttu-id="98405-126">Nenhuma configuração de política de grupo no GPO</span><span class="sxs-lookup"><span data-stu-id="98405-126">No Group Policy settings in GPO</span></span>|



