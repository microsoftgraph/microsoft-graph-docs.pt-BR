---
title: tipo de enum defenderPotentiallyUnwantedAppAction
description: Ação do Defender executar em detectadas aplicativo potencialmente indesejadas (PUA).
ms.openlocfilehash: c786906046d6a35c026da95246016537e4325aab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035199"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="a5d6a-103">tipo de enum defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="a5d6a-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="a5d6a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5d6a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5d6a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5d6a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5d6a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a5d6a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5d6a-107">Ação do Defender executar em detectadas aplicativo potencialmente indesejadas (PUA).</span><span class="sxs-lookup"><span data-stu-id="a5d6a-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>
## <a name="members"></a><span data-ttu-id="a5d6a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a5d6a-108">Members</span></span>
|<span data-ttu-id="a5d6a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a5d6a-109">Member</span></span>|<span data-ttu-id="a5d6a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a5d6a-110">Value</span></span>|<span data-ttu-id="a5d6a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5d6a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5d6a-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a5d6a-112">deviceDefault</span></span>|<span data-ttu-id="a5d6a-113">0</span><span class="sxs-lookup"><span data-stu-id="a5d6a-113">0</span></span>|<span data-ttu-id="a5d6a-114">Proteção de PUA está desativado.</span><span class="sxs-lookup"><span data-stu-id="a5d6a-114">PUA Protection is off.</span></span> <span data-ttu-id="a5d6a-115">Defender não protegerá contra aplicativos potencialmente indesejados.</span><span class="sxs-lookup"><span data-stu-id="a5d6a-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="a5d6a-116">bloquear</span><span class="sxs-lookup"><span data-stu-id="a5d6a-116">block</span></span>|<span data-ttu-id="a5d6a-117">1</span><span class="sxs-lookup"><span data-stu-id="a5d6a-117">1</span></span>|<span data-ttu-id="a5d6a-118">Proteção de PUA é no.</span><span class="sxs-lookup"><span data-stu-id="a5d6a-118">PUA Protection is on.</span></span> <span data-ttu-id="a5d6a-119">Itens detectados serão bloqueados.</span><span class="sxs-lookup"><span data-stu-id="a5d6a-119">Detected items are blocked.</span></span> <span data-ttu-id="a5d6a-120">Eles serão exibidas no histórico junto com outras ameaças.</span><span class="sxs-lookup"><span data-stu-id="a5d6a-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="a5d6a-121">auditoria</span><span class="sxs-lookup"><span data-stu-id="a5d6a-121">audit</span></span>|<span data-ttu-id="a5d6a-122">2</span><span class="sxs-lookup"><span data-stu-id="a5d6a-122">2</span></span>|<span data-ttu-id="a5d6a-123">Modo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a5d6a-123">Audit mode.</span></span> <span data-ttu-id="a5d6a-124">Defender detectar aplicativos potencialmente indesejados, mas não execute nenhuma ações.</span><span class="sxs-lookup"><span data-stu-id="a5d6a-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="a5d6a-125">Você pode revisar as informações sobre aplicativos Defender teria levado ação contra pesquisando criados pelo Defender no evento Visualizador de eventos.</span><span class="sxs-lookup"><span data-stu-id="a5d6a-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





