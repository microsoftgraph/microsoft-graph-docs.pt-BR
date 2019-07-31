---
title: tipo de enumeração edgeKioskModeRestrictionType
description: Especifique como as configurações do Microsoft Edge são restritas com base no modo quiosque.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bbd3d13ad39b6acda5fd67d69c8cb2de2f2e7c55
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001464"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="b77e2-103">tipo de enumeração edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="b77e2-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="b77e2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b77e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b77e2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b77e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b77e2-106">Especifique como as configurações do Microsoft Edge são restritas com base no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b77e2-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="b77e2-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b77e2-107">Members</span></span>
|<span data-ttu-id="b77e2-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b77e2-108">Member</span></span>|<span data-ttu-id="b77e2-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b77e2-109">Value</span></span>|<span data-ttu-id="b77e2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b77e2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b77e2-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b77e2-111">notConfigured</span></span>|<span data-ttu-id="b77e2-112">,0</span><span class="sxs-lookup"><span data-stu-id="b77e2-112">0</span></span>|<span data-ttu-id="b77e2-113">Não configurado (Irrestrito).</span><span class="sxs-lookup"><span data-stu-id="b77e2-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="b77e2-114">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="b77e2-114">digitalSignage</span></span>|<span data-ttu-id="b77e2-115">1</span><span class="sxs-lookup"><span data-stu-id="b77e2-115">1</span></span>|<span data-ttu-id="b77e2-116">Pôsteres/digitais no modo de aplicativo único.</span><span class="sxs-lookup"><span data-stu-id="b77e2-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="b77e2-117">normalmode</span><span class="sxs-lookup"><span data-stu-id="b77e2-117">normalMode</span></span>|<span data-ttu-id="b77e2-118">duas</span><span class="sxs-lookup"><span data-stu-id="b77e2-118">2</span></span>|<span data-ttu-id="b77e2-119">Modo normal (versão completa do Microsoft Edge).</span><span class="sxs-lookup"><span data-stu-id="b77e2-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="b77e2-120">publicBrowsingSingleApp</span><span class="sxs-lookup"><span data-stu-id="b77e2-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="b77e2-121">3D</span><span class="sxs-lookup"><span data-stu-id="b77e2-121">3</span></span>|<span data-ttu-id="b77e2-122">Navegação pública no modo de aplicativo único.</span><span class="sxs-lookup"><span data-stu-id="b77e2-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="b77e2-123">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="b77e2-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="b77e2-124">quatro</span><span class="sxs-lookup"><span data-stu-id="b77e2-124">4</span></span>|<span data-ttu-id="b77e2-125">Navegação pública (InPrivate) no modo de vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="b77e2-125">Public browsing (inPrivate) in multi-app mode.</span></span>|





