---
title: tipo de enumeração defenderPotentiallyUnwantedAppAction
description: Ação do defender a ser executada em aplicativo potencialmente inDesejado (PUA).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1949ec58c7cfd2d896308f740b7eca16f2646b3e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534805"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="a89ef-103">tipo de enumeração defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="a89ef-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="a89ef-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a89ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a89ef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a89ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a89ef-106">Ação do defender a ser executada em aplicativo potencialmente inDesejado (PUA).</span><span class="sxs-lookup"><span data-stu-id="a89ef-106">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="a89ef-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a89ef-107">Members</span></span>
|<span data-ttu-id="a89ef-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a89ef-108">Member</span></span>|<span data-ttu-id="a89ef-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a89ef-109">Value</span></span>|<span data-ttu-id="a89ef-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a89ef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a89ef-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a89ef-111">deviceDefault</span></span>|<span data-ttu-id="a89ef-112">,0</span><span class="sxs-lookup"><span data-stu-id="a89ef-112">0</span></span>|<span data-ttu-id="a89ef-113">A proteção do PUA está desativada.</span><span class="sxs-lookup"><span data-stu-id="a89ef-113">PUA Protection is off.</span></span> <span data-ttu-id="a89ef-114">O defender não protegerá contra aplicativos potencialmente indesejados.</span><span class="sxs-lookup"><span data-stu-id="a89ef-114">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="a89ef-115">Larga</span><span class="sxs-lookup"><span data-stu-id="a89ef-115">block</span></span>|<span data-ttu-id="a89ef-116">1 </span><span class="sxs-lookup"><span data-stu-id="a89ef-116">1</span></span>|<span data-ttu-id="a89ef-117">A proteção do PUA está ativada.</span><span class="sxs-lookup"><span data-stu-id="a89ef-117">PUA Protection is on.</span></span> <span data-ttu-id="a89ef-118">Os itens detectados são bloqueados.</span><span class="sxs-lookup"><span data-stu-id="a89ef-118">Detected items are blocked.</span></span> <span data-ttu-id="a89ef-119">Eles serão mostrados em histórico junto com outras ameaças.</span><span class="sxs-lookup"><span data-stu-id="a89ef-119">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="a89ef-120">Faça</span><span class="sxs-lookup"><span data-stu-id="a89ef-120">audit</span></span>|<span data-ttu-id="a89ef-121">2 </span><span class="sxs-lookup"><span data-stu-id="a89ef-121">2</span></span>|<span data-ttu-id="a89ef-122">Modo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a89ef-122">Audit mode.</span></span> <span data-ttu-id="a89ef-123">O defender detectará aplicativos potencialmente indesejados, mas não realizará ações.</span><span class="sxs-lookup"><span data-stu-id="a89ef-123">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="a89ef-124">Você pode revisar as informações sobre os aplicativos que o defender teria feito com a pesquisa de eventos criados pelo defender no Visualizador de eventos.</span><span class="sxs-lookup"><span data-stu-id="a89ef-124">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





