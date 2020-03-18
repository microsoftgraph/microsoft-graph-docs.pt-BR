---
title: tipo de enumeração edgeKioskModeRestrictionType
description: Especifique como as configurações do Microsoft Edge são restritas com base no modo quiosque.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 402feb76fbb95664f5b4fe8190dfb71504db0abf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791874"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="68c1f-103">tipo de enumeração edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="68c1f-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="68c1f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="68c1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68c1f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68c1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68c1f-106">Especifique como as configurações do Microsoft Edge são restritas com base no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="68c1f-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="68c1f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="68c1f-107">Members</span></span>
|<span data-ttu-id="68c1f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="68c1f-108">Member</span></span>|<span data-ttu-id="68c1f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="68c1f-109">Value</span></span>|<span data-ttu-id="68c1f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="68c1f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68c1f-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="68c1f-111">notConfigured</span></span>|<span data-ttu-id="68c1f-112">,0</span><span class="sxs-lookup"><span data-stu-id="68c1f-112">0</span></span>|<span data-ttu-id="68c1f-113">Não configurado (Irrestrito).</span><span class="sxs-lookup"><span data-stu-id="68c1f-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="68c1f-114">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="68c1f-114">digitalSignage</span></span>|<span data-ttu-id="68c1f-115">1</span><span class="sxs-lookup"><span data-stu-id="68c1f-115">1</span></span>|<span data-ttu-id="68c1f-116">Pôsteres/digitais no modo de aplicativo único.</span><span class="sxs-lookup"><span data-stu-id="68c1f-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="68c1f-117">normalmode</span><span class="sxs-lookup"><span data-stu-id="68c1f-117">normalMode</span></span>|<span data-ttu-id="68c1f-118">duas</span><span class="sxs-lookup"><span data-stu-id="68c1f-118">2</span></span>|<span data-ttu-id="68c1f-119">Modo normal (versão completa do Microsoft Edge).</span><span class="sxs-lookup"><span data-stu-id="68c1f-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="68c1f-120">publicBrowsingSingleApp</span><span class="sxs-lookup"><span data-stu-id="68c1f-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="68c1f-121">3D</span><span class="sxs-lookup"><span data-stu-id="68c1f-121">3</span></span>|<span data-ttu-id="68c1f-122">Navegação pública no modo de aplicativo único.</span><span class="sxs-lookup"><span data-stu-id="68c1f-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="68c1f-123">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="68c1f-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="68c1f-124">4 </span><span class="sxs-lookup"><span data-stu-id="68c1f-124">4</span></span>|<span data-ttu-id="68c1f-125">Navegação pública (InPrivate) no modo de vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="68c1f-125">Public browsing (inPrivate) in multi-app mode.</span></span>|



