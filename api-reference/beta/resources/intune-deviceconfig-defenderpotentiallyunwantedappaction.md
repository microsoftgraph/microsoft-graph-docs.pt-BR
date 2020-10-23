---
title: tipo de enumeração defenderPotentiallyUnwantedAppAction
description: Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2919edb11cc29f8a78d3bde32808f285eef25b4c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696353"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="7869c-103">tipo de enumeração defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="7869c-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

<span data-ttu-id="7869c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7869c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7869c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7869c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7869c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7869c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7869c-107">Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).</span><span class="sxs-lookup"><span data-stu-id="7869c-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="7869c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="7869c-108">Members</span></span>
|<span data-ttu-id="7869c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="7869c-109">Member</span></span>|<span data-ttu-id="7869c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="7869c-110">Value</span></span>|<span data-ttu-id="7869c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7869c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7869c-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="7869c-112">deviceDefault</span></span>|<span data-ttu-id="7869c-113">,0</span><span class="sxs-lookup"><span data-stu-id="7869c-113">0</span></span>|<span data-ttu-id="7869c-114">A proteção do PUA está desativada.</span><span class="sxs-lookup"><span data-stu-id="7869c-114">PUA Protection is off.</span></span> <span data-ttu-id="7869c-115">O defender não protegerá contra aplicativos potencialmente indesejados.</span><span class="sxs-lookup"><span data-stu-id="7869c-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="7869c-116">Larga</span><span class="sxs-lookup"><span data-stu-id="7869c-116">block</span></span>|<span data-ttu-id="7869c-117">1</span><span class="sxs-lookup"><span data-stu-id="7869c-117">1</span></span>|<span data-ttu-id="7869c-118">A proteção do PUA está ativada.</span><span class="sxs-lookup"><span data-stu-id="7869c-118">PUA Protection is on.</span></span> <span data-ttu-id="7869c-119">Os itens detectados são bloqueados.</span><span class="sxs-lookup"><span data-stu-id="7869c-119">Detected items are blocked.</span></span> <span data-ttu-id="7869c-120">Eles serão mostrados em histórico junto com outras ameaças.</span><span class="sxs-lookup"><span data-stu-id="7869c-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="7869c-121">Faça</span><span class="sxs-lookup"><span data-stu-id="7869c-121">audit</span></span>|<span data-ttu-id="7869c-122">duas</span><span class="sxs-lookup"><span data-stu-id="7869c-122">2</span></span>|<span data-ttu-id="7869c-123">Modo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="7869c-123">Audit mode.</span></span> <span data-ttu-id="7869c-124">O defender detectará aplicativos potencialmente indesejados, mas não realizará ações.</span><span class="sxs-lookup"><span data-stu-id="7869c-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="7869c-125">Você pode revisar as informações sobre os aplicativos que o defender teria feito com a pesquisa de eventos criados pelo defender no Visualizador de eventos.</span><span class="sxs-lookup"><span data-stu-id="7869c-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





