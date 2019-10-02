---
title: tipo de enumeração managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4e16eb22dfe09135857eca5a936df4b276e465b2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356412"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="8e09f-103">tipo de enumeração managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="8e09f-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="8e09f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e09f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e09f-105">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="8e09f-105">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="8e09f-106">Membros</span><span class="sxs-lookup"><span data-stu-id="8e09f-106">Members</span></span>
|<span data-ttu-id="8e09f-107">Membro</span><span class="sxs-lookup"><span data-stu-id="8e09f-107">Member</span></span>|<span data-ttu-id="8e09f-108">Valor</span><span class="sxs-lookup"><span data-stu-id="8e09f-108">Value</span></span>|<span data-ttu-id="8e09f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e09f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e09f-110">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="8e09f-110">allApps</span></span>|<span data-ttu-id="8e09f-111">,0</span><span class="sxs-lookup"><span data-stu-id="8e09f-111">0</span></span>|<span data-ttu-id="8e09f-112">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="8e09f-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="8e09f-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="8e09f-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="8e09f-114">1</span><span class="sxs-lookup"><span data-stu-id="8e09f-114">1</span></span>|<span data-ttu-id="8e09f-115">O compartilhamento é permitido entre todos os aplicativos gerenciados com colar ativado</span><span class="sxs-lookup"><span data-stu-id="8e09f-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="8e09f-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="8e09f-116">managedApps</span></span>|<span data-ttu-id="8e09f-117">duas</span><span class="sxs-lookup"><span data-stu-id="8e09f-117">2</span></span>|<span data-ttu-id="8e09f-118">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="8e09f-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="8e09f-119">bloqueou</span><span class="sxs-lookup"><span data-stu-id="8e09f-119">blocked</span></span>|<span data-ttu-id="8e09f-120">3D</span><span class="sxs-lookup"><span data-stu-id="8e09f-120">3</span></span>|<span data-ttu-id="8e09f-121">O compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8e09f-121">Sharing between apps is disabled</span></span>|




