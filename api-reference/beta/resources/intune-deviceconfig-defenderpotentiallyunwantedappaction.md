---
title: tipo de enumeração defenderPotentiallyUnwantedAppAction
description: Ação do defender a ser executada em aplicativo potencialmente inDesejado (PUA).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02ac5da63c2787c2b87479a23899c9d2980c54c4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173350"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="48d89-103">tipo de enumeração defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="48d89-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="48d89-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48d89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48d89-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48d89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48d89-106">Ação do defender a ser executada em aplicativo potencialmente inDesejado (PUA).</span><span class="sxs-lookup"><span data-stu-id="48d89-106">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="48d89-107">Membros</span><span class="sxs-lookup"><span data-stu-id="48d89-107">Members</span></span>
|<span data-ttu-id="48d89-108">Membro</span><span class="sxs-lookup"><span data-stu-id="48d89-108">Member</span></span>|<span data-ttu-id="48d89-109">Valor</span><span class="sxs-lookup"><span data-stu-id="48d89-109">Value</span></span>|<span data-ttu-id="48d89-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="48d89-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48d89-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="48d89-111">deviceDefault</span></span>|<span data-ttu-id="48d89-112">,0</span><span class="sxs-lookup"><span data-stu-id="48d89-112">0</span></span>|<span data-ttu-id="48d89-113">A proteção do PUA está desativada.</span><span class="sxs-lookup"><span data-stu-id="48d89-113">PUA Protection is off.</span></span> <span data-ttu-id="48d89-114">O defender não protegerá contra aplicativos potencialmente indesejados.</span><span class="sxs-lookup"><span data-stu-id="48d89-114">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="48d89-115">Larga</span><span class="sxs-lookup"><span data-stu-id="48d89-115">block</span></span>|<span data-ttu-id="48d89-116">1</span><span class="sxs-lookup"><span data-stu-id="48d89-116">1</span></span>|<span data-ttu-id="48d89-117">A proteção do PUA está ativada.</span><span class="sxs-lookup"><span data-stu-id="48d89-117">PUA Protection is on.</span></span> <span data-ttu-id="48d89-118">Os itens detectados são bloqueados.</span><span class="sxs-lookup"><span data-stu-id="48d89-118">Detected items are blocked.</span></span> <span data-ttu-id="48d89-119">Eles serão mostrados em histórico junto com outras ameaças.</span><span class="sxs-lookup"><span data-stu-id="48d89-119">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="48d89-120">Faça</span><span class="sxs-lookup"><span data-stu-id="48d89-120">audit</span></span>|<span data-ttu-id="48d89-121">duas</span><span class="sxs-lookup"><span data-stu-id="48d89-121">2</span></span>|<span data-ttu-id="48d89-122">Modo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="48d89-122">Audit mode.</span></span> <span data-ttu-id="48d89-123">O defender detectará aplicativos potencialmente indesejados, mas não realizará ações.</span><span class="sxs-lookup"><span data-stu-id="48d89-123">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="48d89-124">Você pode revisar as informações sobre os aplicativos que o defender teria feito com a pesquisa de eventos criados pelo defender no Visualizador de eventos.</span><span class="sxs-lookup"><span data-stu-id="48d89-124">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|




