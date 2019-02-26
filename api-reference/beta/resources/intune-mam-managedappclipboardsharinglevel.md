---
title: tipo de enumeração managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 352a801c53acd487fdac0206eca828461d35bf68
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148346"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="b11f2-103">tipo de enumeração managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="b11f2-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="b11f2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b11f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b11f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b11f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b11f2-106">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="b11f2-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="b11f2-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b11f2-107">Members</span></span>
|<span data-ttu-id="b11f2-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b11f2-108">Member</span></span>|<span data-ttu-id="b11f2-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b11f2-109">Value</span></span>|<span data-ttu-id="b11f2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b11f2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b11f2-111">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="b11f2-111">allApps</span></span>|<span data-ttu-id="b11f2-112">,0</span><span class="sxs-lookup"><span data-stu-id="b11f2-112">0</span></span>|<span data-ttu-id="b11f2-113">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="b11f2-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="b11f2-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="b11f2-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="b11f2-115">1</span><span class="sxs-lookup"><span data-stu-id="b11f2-115">1</span></span>|<span data-ttu-id="b11f2-116">O compartilhamento é permitido entre todos os aplicativos gerenciados com colar ativado</span><span class="sxs-lookup"><span data-stu-id="b11f2-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="b11f2-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="b11f2-117">managedApps</span></span>|<span data-ttu-id="b11f2-118">duas</span><span class="sxs-lookup"><span data-stu-id="b11f2-118">2</span></span>|<span data-ttu-id="b11f2-119">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="b11f2-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="b11f2-120">bloqueou</span><span class="sxs-lookup"><span data-stu-id="b11f2-120">blocked</span></span>|<span data-ttu-id="b11f2-121">3D</span><span class="sxs-lookup"><span data-stu-id="b11f2-121">3</span></span>|<span data-ttu-id="b11f2-122">O compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="b11f2-122">Sharing between apps is disabled</span></span>|




