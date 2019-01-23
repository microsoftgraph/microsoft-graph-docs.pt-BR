---
title: tipo de enum defenderPotentiallyUnwantedAppAction
description: Ação do Defender executar em detectadas aplicativo potencialmente indesejadas (PUA).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2ace0cc29ad284cde63b7e4934fb8cb395f27bbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422751"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="faad7-103">tipo de enum defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="faad7-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="faad7-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="faad7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="faad7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="faad7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="faad7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="faad7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faad7-107">Ação do Defender executar em detectadas aplicativo potencialmente indesejadas (PUA).</span><span class="sxs-lookup"><span data-stu-id="faad7-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="faad7-108">Membros</span><span class="sxs-lookup"><span data-stu-id="faad7-108">Members</span></span>
|<span data-ttu-id="faad7-109">Membro</span><span class="sxs-lookup"><span data-stu-id="faad7-109">Member</span></span>|<span data-ttu-id="faad7-110">Valor</span><span class="sxs-lookup"><span data-stu-id="faad7-110">Value</span></span>|<span data-ttu-id="faad7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="faad7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faad7-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="faad7-112">deviceDefault</span></span>|<span data-ttu-id="faad7-113">0</span><span class="sxs-lookup"><span data-stu-id="faad7-113">0</span></span>|<span data-ttu-id="faad7-114">Proteção de PUA está desativado.</span><span class="sxs-lookup"><span data-stu-id="faad7-114">PUA Protection is off.</span></span> <span data-ttu-id="faad7-115">Defender não protegerá contra aplicativos potencialmente indesejados.</span><span class="sxs-lookup"><span data-stu-id="faad7-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="faad7-116">bloquear</span><span class="sxs-lookup"><span data-stu-id="faad7-116">block</span></span>|<span data-ttu-id="faad7-117">1</span><span class="sxs-lookup"><span data-stu-id="faad7-117">1</span></span>|<span data-ttu-id="faad7-118">Proteção de PUA é no.</span><span class="sxs-lookup"><span data-stu-id="faad7-118">PUA Protection is on.</span></span> <span data-ttu-id="faad7-119">Itens detectados serão bloqueados.</span><span class="sxs-lookup"><span data-stu-id="faad7-119">Detected items are blocked.</span></span> <span data-ttu-id="faad7-120">Eles serão exibidas no histórico junto com outras ameaças.</span><span class="sxs-lookup"><span data-stu-id="faad7-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="faad7-121">auditoria</span><span class="sxs-lookup"><span data-stu-id="faad7-121">audit</span></span>|<span data-ttu-id="faad7-122">2</span><span class="sxs-lookup"><span data-stu-id="faad7-122">2</span></span>|<span data-ttu-id="faad7-123">Modo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="faad7-123">Audit mode.</span></span> <span data-ttu-id="faad7-124">Defender detectar aplicativos potencialmente indesejados, mas não execute nenhuma ações.</span><span class="sxs-lookup"><span data-stu-id="faad7-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="faad7-125">Você pode revisar as informações sobre aplicativos Defender teria levado ação contra pesquisando criados pelo Defender no evento Visualizador de eventos.</span><span class="sxs-lookup"><span data-stu-id="faad7-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|




