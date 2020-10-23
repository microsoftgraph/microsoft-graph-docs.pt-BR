---
title: tipo de enumeração edgeKioskModeRestrictionType
description: Especifique como as configurações do Microsoft Edge são restritas com base no modo quiosque.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 98d360d220df9b94f1a13194885d576bcdf362da
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732569"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="ff014-103">tipo de enumeração edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="ff014-103">edgeKioskModeRestrictionType enum type</span></span>

<span data-ttu-id="ff014-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff014-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff014-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff014-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff014-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff014-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff014-107">Especifique como as configurações do Microsoft Edge são restritas com base no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ff014-107">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="ff014-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ff014-108">Members</span></span>
|<span data-ttu-id="ff014-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ff014-109">Member</span></span>|<span data-ttu-id="ff014-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ff014-110">Value</span></span>|<span data-ttu-id="ff014-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff014-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff014-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ff014-112">notConfigured</span></span>|<span data-ttu-id="ff014-113">,0</span><span class="sxs-lookup"><span data-stu-id="ff014-113">0</span></span>|<span data-ttu-id="ff014-114">Não configurado (Irrestrito).</span><span class="sxs-lookup"><span data-stu-id="ff014-114">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="ff014-115">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="ff014-115">digitalSignage</span></span>|<span data-ttu-id="ff014-116">1</span><span class="sxs-lookup"><span data-stu-id="ff014-116">1</span></span>|<span data-ttu-id="ff014-117">Pôsteres/digitais no modo de aplicativo único.</span><span class="sxs-lookup"><span data-stu-id="ff014-117">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="ff014-118">normalmode</span><span class="sxs-lookup"><span data-stu-id="ff014-118">normalMode</span></span>|<span data-ttu-id="ff014-119">duas</span><span class="sxs-lookup"><span data-stu-id="ff014-119">2</span></span>|<span data-ttu-id="ff014-120">Modo normal (versão completa do Microsoft Edge).</span><span class="sxs-lookup"><span data-stu-id="ff014-120">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="ff014-121">publicBrowsingSingleApp</span><span class="sxs-lookup"><span data-stu-id="ff014-121">publicBrowsingSingleApp</span></span>|<span data-ttu-id="ff014-122">3D</span><span class="sxs-lookup"><span data-stu-id="ff014-122">3</span></span>|<span data-ttu-id="ff014-123">Navegação pública no modo de aplicativo único.</span><span class="sxs-lookup"><span data-stu-id="ff014-123">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="ff014-124">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="ff014-124">publicBrowsingMultiApp</span></span>|<span data-ttu-id="ff014-125">4 </span><span class="sxs-lookup"><span data-stu-id="ff014-125">4</span></span>|<span data-ttu-id="ff014-126">Navegação pública (InPrivate) no modo de vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ff014-126">Public browsing (inPrivate) in multi-app mode.</span></span>|





