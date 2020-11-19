---
title: tipo de enumeração defenderPotentiallyUnwantedAppAction
description: Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: aad2c9e37dfe3a3069caad25c7917a864c65a194
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256509"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="59a03-103">tipo de enumeração defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="59a03-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

<span data-ttu-id="59a03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59a03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59a03-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59a03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59a03-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59a03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59a03-107">Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).</span><span class="sxs-lookup"><span data-stu-id="59a03-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="59a03-108">Membros</span><span class="sxs-lookup"><span data-stu-id="59a03-108">Members</span></span>
|<span data-ttu-id="59a03-109">Membro</span><span class="sxs-lookup"><span data-stu-id="59a03-109">Member</span></span>|<span data-ttu-id="59a03-110">Valor</span><span class="sxs-lookup"><span data-stu-id="59a03-110">Value</span></span>|<span data-ttu-id="59a03-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="59a03-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59a03-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="59a03-112">deviceDefault</span></span>|<span data-ttu-id="59a03-113">,0</span><span class="sxs-lookup"><span data-stu-id="59a03-113">0</span></span>|<span data-ttu-id="59a03-114">A proteção do PUA está desativada.</span><span class="sxs-lookup"><span data-stu-id="59a03-114">PUA Protection is off.</span></span> <span data-ttu-id="59a03-115">O defender não protegerá contra aplicativos potencialmente indesejados.</span><span class="sxs-lookup"><span data-stu-id="59a03-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="59a03-116">Larga</span><span class="sxs-lookup"><span data-stu-id="59a03-116">block</span></span>|<span data-ttu-id="59a03-117">1</span><span class="sxs-lookup"><span data-stu-id="59a03-117">1</span></span>|<span data-ttu-id="59a03-118">A proteção do PUA está ativada.</span><span class="sxs-lookup"><span data-stu-id="59a03-118">PUA Protection is on.</span></span> <span data-ttu-id="59a03-119">Os itens detectados são bloqueados.</span><span class="sxs-lookup"><span data-stu-id="59a03-119">Detected items are blocked.</span></span> <span data-ttu-id="59a03-120">Eles serão mostrados em histórico junto com outras ameaças.</span><span class="sxs-lookup"><span data-stu-id="59a03-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="59a03-121">Faça</span><span class="sxs-lookup"><span data-stu-id="59a03-121">audit</span></span>|<span data-ttu-id="59a03-122">duas</span><span class="sxs-lookup"><span data-stu-id="59a03-122">2</span></span>|<span data-ttu-id="59a03-123">Modo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="59a03-123">Audit mode.</span></span> <span data-ttu-id="59a03-124">O defender detectará aplicativos potencialmente indesejados, mas não realizará ações.</span><span class="sxs-lookup"><span data-stu-id="59a03-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="59a03-125">Você pode revisar as informações sobre os aplicativos que o defender teria feito com a pesquisa de eventos criados pelo defender no Visualizador de eventos.</span><span class="sxs-lookup"><span data-stu-id="59a03-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|




