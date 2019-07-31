---
title: tipo de enumeração defenderPotentiallyUnwantedAppAction
description: Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a05aafa9a14399191adedc6c083ee371fe090a7f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970931"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="d0870-103">tipo de enumeração defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="d0870-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="d0870-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d0870-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0870-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0870-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0870-106">Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).</span><span class="sxs-lookup"><span data-stu-id="d0870-106">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="d0870-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d0870-107">Members</span></span>
|<span data-ttu-id="d0870-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d0870-108">Member</span></span>|<span data-ttu-id="d0870-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d0870-109">Value</span></span>|<span data-ttu-id="d0870-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0870-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0870-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d0870-111">deviceDefault</span></span>|<span data-ttu-id="d0870-112">,0</span><span class="sxs-lookup"><span data-stu-id="d0870-112">0</span></span>|<span data-ttu-id="d0870-113">A proteção do PUA está desativada.</span><span class="sxs-lookup"><span data-stu-id="d0870-113">PUA Protection is off.</span></span> <span data-ttu-id="d0870-114">O defender não protegerá contra aplicativos potencialmente indesejados.</span><span class="sxs-lookup"><span data-stu-id="d0870-114">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="d0870-115">Larga</span><span class="sxs-lookup"><span data-stu-id="d0870-115">block</span></span>|<span data-ttu-id="d0870-116">1</span><span class="sxs-lookup"><span data-stu-id="d0870-116">1</span></span>|<span data-ttu-id="d0870-117">A proteção do PUA está ativada.</span><span class="sxs-lookup"><span data-stu-id="d0870-117">PUA Protection is on.</span></span> <span data-ttu-id="d0870-118">Os itens detectados são bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d0870-118">Detected items are blocked.</span></span> <span data-ttu-id="d0870-119">Eles serão mostrados em histórico junto com outras ameaças.</span><span class="sxs-lookup"><span data-stu-id="d0870-119">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="d0870-120">Faça</span><span class="sxs-lookup"><span data-stu-id="d0870-120">audit</span></span>|<span data-ttu-id="d0870-121">duas</span><span class="sxs-lookup"><span data-stu-id="d0870-121">2</span></span>|<span data-ttu-id="d0870-122">Modo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="d0870-122">Audit mode.</span></span> <span data-ttu-id="d0870-123">O defender detectará aplicativos potencialmente indesejados, mas não realizará ações.</span><span class="sxs-lookup"><span data-stu-id="d0870-123">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="d0870-124">Você pode revisar as informações sobre os aplicativos que o defender teria feito com a pesquisa de eventos criados pelo defender no Visualizador de eventos.</span><span class="sxs-lookup"><span data-stu-id="d0870-124">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





