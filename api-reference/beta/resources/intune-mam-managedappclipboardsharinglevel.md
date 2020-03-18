---
title: tipo de enumeração managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5f6153eeb4b76af9d8974b715b7c6342c646ba6e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782241"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="d9775-103">tipo de enumeração managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="d9775-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="d9775-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9775-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9775-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9775-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9775-106">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="d9775-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="d9775-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d9775-107">Members</span></span>
|<span data-ttu-id="d9775-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d9775-108">Member</span></span>|<span data-ttu-id="d9775-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d9775-109">Value</span></span>|<span data-ttu-id="d9775-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9775-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9775-111">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="d9775-111">allApps</span></span>|<span data-ttu-id="d9775-112">,0</span><span class="sxs-lookup"><span data-stu-id="d9775-112">0</span></span>|<span data-ttu-id="d9775-113">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="d9775-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="d9775-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="d9775-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="d9775-115">1</span><span class="sxs-lookup"><span data-stu-id="d9775-115">1</span></span>|<span data-ttu-id="d9775-116">O compartilhamento é permitido entre todos os aplicativos gerenciados com colar ativado</span><span class="sxs-lookup"><span data-stu-id="d9775-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="d9775-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="d9775-117">managedApps</span></span>|<span data-ttu-id="d9775-118">duas</span><span class="sxs-lookup"><span data-stu-id="d9775-118">2</span></span>|<span data-ttu-id="d9775-119">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="d9775-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="d9775-120">bloqueou</span><span class="sxs-lookup"><span data-stu-id="d9775-120">blocked</span></span>|<span data-ttu-id="d9775-121">3D</span><span class="sxs-lookup"><span data-stu-id="d9775-121">3</span></span>|<span data-ttu-id="d9775-122">O compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="d9775-122">Sharing between apps is disabled</span></span>|



