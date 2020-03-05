---
title: tipo de enumeração edgeKioskModeRestrictionType
description: Especifique como as configurações do Microsoft Edge são restritas com base no modo quiosque.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 929e74097d329f2d6932ae3aadaa001258dbd2fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530057"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="9ab59-103">tipo de enumeração edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="9ab59-103">edgeKioskModeRestrictionType enum type</span></span>

<span data-ttu-id="9ab59-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9ab59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ab59-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ab59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ab59-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ab59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ab59-107">Especifique como as configurações do Microsoft Edge são restritas com base no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="9ab59-107">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="9ab59-108">Membros</span><span class="sxs-lookup"><span data-stu-id="9ab59-108">Members</span></span>
|<span data-ttu-id="9ab59-109">Membro</span><span class="sxs-lookup"><span data-stu-id="9ab59-109">Member</span></span>|<span data-ttu-id="9ab59-110">Valor</span><span class="sxs-lookup"><span data-stu-id="9ab59-110">Value</span></span>|<span data-ttu-id="9ab59-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ab59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ab59-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9ab59-112">notConfigured</span></span>|<span data-ttu-id="9ab59-113">,0</span><span class="sxs-lookup"><span data-stu-id="9ab59-113">0</span></span>|<span data-ttu-id="9ab59-114">Não configurado (Irrestrito).</span><span class="sxs-lookup"><span data-stu-id="9ab59-114">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="9ab59-115">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="9ab59-115">digitalSignage</span></span>|<span data-ttu-id="9ab59-116">1 </span><span class="sxs-lookup"><span data-stu-id="9ab59-116">1</span></span>|<span data-ttu-id="9ab59-117">Pôsteres/digitais no modo de aplicativo único.</span><span class="sxs-lookup"><span data-stu-id="9ab59-117">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="9ab59-118">normalmode</span><span class="sxs-lookup"><span data-stu-id="9ab59-118">normalMode</span></span>|<span data-ttu-id="9ab59-119">2 </span><span class="sxs-lookup"><span data-stu-id="9ab59-119">2</span></span>|<span data-ttu-id="9ab59-120">Modo normal (versão completa do Microsoft Edge).</span><span class="sxs-lookup"><span data-stu-id="9ab59-120">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="9ab59-121">publicBrowsingSingleApp</span><span class="sxs-lookup"><span data-stu-id="9ab59-121">publicBrowsingSingleApp</span></span>|<span data-ttu-id="9ab59-122">3 </span><span class="sxs-lookup"><span data-stu-id="9ab59-122">3</span></span>|<span data-ttu-id="9ab59-123">Navegação pública no modo de aplicativo único.</span><span class="sxs-lookup"><span data-stu-id="9ab59-123">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="9ab59-124">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="9ab59-124">publicBrowsingMultiApp</span></span>|<span data-ttu-id="9ab59-125">4 </span><span class="sxs-lookup"><span data-stu-id="9ab59-125">4</span></span>|<span data-ttu-id="9ab59-126">Navegação pública (InPrivate) no modo de vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="9ab59-126">Public browsing (inPrivate) in multi-app mode.</span></span>|



