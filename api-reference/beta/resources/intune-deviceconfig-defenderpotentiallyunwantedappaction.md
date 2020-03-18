---
title: tipo de enumeração defenderPotentiallyUnwantedAppAction
description: Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0c99cf04b217239fb1a06b2a6c26dcacc6c61cf7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794463"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="7753d-103">tipo de enumeração defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="7753d-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="7753d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7753d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7753d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7753d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7753d-106">Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).</span><span class="sxs-lookup"><span data-stu-id="7753d-106">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="7753d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="7753d-107">Members</span></span>
|<span data-ttu-id="7753d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="7753d-108">Member</span></span>|<span data-ttu-id="7753d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="7753d-109">Value</span></span>|<span data-ttu-id="7753d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7753d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7753d-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="7753d-111">deviceDefault</span></span>|<span data-ttu-id="7753d-112">,0</span><span class="sxs-lookup"><span data-stu-id="7753d-112">0</span></span>|<span data-ttu-id="7753d-113">A proteção do PUA está desativada.</span><span class="sxs-lookup"><span data-stu-id="7753d-113">PUA Protection is off.</span></span> <span data-ttu-id="7753d-114">O defender não protegerá contra aplicativos potencialmente indesejados.</span><span class="sxs-lookup"><span data-stu-id="7753d-114">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="7753d-115">Larga</span><span class="sxs-lookup"><span data-stu-id="7753d-115">block</span></span>|<span data-ttu-id="7753d-116">1</span><span class="sxs-lookup"><span data-stu-id="7753d-116">1</span></span>|<span data-ttu-id="7753d-117">A proteção do PUA está ativada.</span><span class="sxs-lookup"><span data-stu-id="7753d-117">PUA Protection is on.</span></span> <span data-ttu-id="7753d-118">Os itens detectados são bloqueados.</span><span class="sxs-lookup"><span data-stu-id="7753d-118">Detected items are blocked.</span></span> <span data-ttu-id="7753d-119">Eles serão mostrados em histórico junto com outras ameaças.</span><span class="sxs-lookup"><span data-stu-id="7753d-119">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="7753d-120">Faça</span><span class="sxs-lookup"><span data-stu-id="7753d-120">audit</span></span>|<span data-ttu-id="7753d-121">duas</span><span class="sxs-lookup"><span data-stu-id="7753d-121">2</span></span>|<span data-ttu-id="7753d-122">Modo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="7753d-122">Audit mode.</span></span> <span data-ttu-id="7753d-123">O defender detectará aplicativos potencialmente indesejados, mas não realizará ações.</span><span class="sxs-lookup"><span data-stu-id="7753d-123">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="7753d-124">Você pode revisar as informações sobre os aplicativos que o defender teria feito com a pesquisa de eventos criados pelo defender no Visualizador de eventos.</span><span class="sxs-lookup"><span data-stu-id="7753d-124">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|



