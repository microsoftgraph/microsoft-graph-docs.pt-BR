---
title: tipo de enumeração managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 339dc8a824073f609ee580042895bd3a59f58e43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998433"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="80d42-103">tipo de enumeração managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="80d42-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="80d42-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80d42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80d42-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80d42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80d42-106">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="80d42-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="80d42-107">Membros</span><span class="sxs-lookup"><span data-stu-id="80d42-107">Members</span></span>
|<span data-ttu-id="80d42-108">Membro</span><span class="sxs-lookup"><span data-stu-id="80d42-108">Member</span></span>|<span data-ttu-id="80d42-109">Valor</span><span class="sxs-lookup"><span data-stu-id="80d42-109">Value</span></span>|<span data-ttu-id="80d42-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="80d42-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80d42-111">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="80d42-111">allApps</span></span>|<span data-ttu-id="80d42-112">,0</span><span class="sxs-lookup"><span data-stu-id="80d42-112">0</span></span>|<span data-ttu-id="80d42-113">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="80d42-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="80d42-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="80d42-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="80d42-115">1</span><span class="sxs-lookup"><span data-stu-id="80d42-115">1</span></span>|<span data-ttu-id="80d42-116">O compartilhamento é permitido entre todos os aplicativos gerenciados com colar ativado</span><span class="sxs-lookup"><span data-stu-id="80d42-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="80d42-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="80d42-117">managedApps</span></span>|<span data-ttu-id="80d42-118">duas</span><span class="sxs-lookup"><span data-stu-id="80d42-118">2</span></span>|<span data-ttu-id="80d42-119">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="80d42-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="80d42-120">bloqueou</span><span class="sxs-lookup"><span data-stu-id="80d42-120">blocked</span></span>|<span data-ttu-id="80d42-121">3D</span><span class="sxs-lookup"><span data-stu-id="80d42-121">3</span></span>|<span data-ttu-id="80d42-122">O compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="80d42-122">Sharing between apps is disabled</span></span>|





