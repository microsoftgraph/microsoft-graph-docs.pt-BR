---
title: tipo de enumeração edgeKioskModeRestrictionType
description: Especifique como as configurações do Microsoft Edge são restritas com base no modo quiosque.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74b03555456c058411c9a50c7392f29fe60d3aed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524509"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="c9b4c-103">tipo de enumeração edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="c9b4c-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="c9b4c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c9b4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9b4c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9b4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9b4c-106">Especifique como as configurações do Microsoft Edge são restritas com base no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="c9b4c-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="c9b4c-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c9b4c-107">Members</span></span>
|<span data-ttu-id="c9b4c-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c9b4c-108">Member</span></span>|<span data-ttu-id="c9b4c-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c9b4c-109">Value</span></span>|<span data-ttu-id="c9b4c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9b4c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9b4c-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c9b4c-111">notConfigured</span></span>|<span data-ttu-id="c9b4c-112">,0</span><span class="sxs-lookup"><span data-stu-id="c9b4c-112">0</span></span>|<span data-ttu-id="c9b4c-113">Não configurado (Irrestrito).</span><span class="sxs-lookup"><span data-stu-id="c9b4c-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="c9b4c-114">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="c9b4c-114">digitalSignage</span></span>|<span data-ttu-id="c9b4c-115">1 </span><span class="sxs-lookup"><span data-stu-id="c9b4c-115">1</span></span>|<span data-ttu-id="c9b4c-116">Pôsteres/digitais no modo de aplicativo único.</span><span class="sxs-lookup"><span data-stu-id="c9b4c-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="c9b4c-117">normalmode</span><span class="sxs-lookup"><span data-stu-id="c9b4c-117">normalMode</span></span>|<span data-ttu-id="c9b4c-118">2 </span><span class="sxs-lookup"><span data-stu-id="c9b4c-118">2</span></span>|<span data-ttu-id="c9b4c-119">Modo normal (versão completa do Microsoft Edge).</span><span class="sxs-lookup"><span data-stu-id="c9b4c-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="c9b4c-120">publicBrowsingSingleApp</span><span class="sxs-lookup"><span data-stu-id="c9b4c-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="c9b4c-121">3 </span><span class="sxs-lookup"><span data-stu-id="c9b4c-121">3</span></span>|<span data-ttu-id="c9b4c-122">Navegação pública no modo de aplicativo único.</span><span class="sxs-lookup"><span data-stu-id="c9b4c-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="c9b4c-123">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="c9b4c-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="c9b4c-124">4 </span><span class="sxs-lookup"><span data-stu-id="c9b4c-124">4</span></span>|<span data-ttu-id="c9b4c-125">Navegação pública (InPrivate) no modo de vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="c9b4c-125">Public browsing (inPrivate) in multi-app mode.</span></span>|





