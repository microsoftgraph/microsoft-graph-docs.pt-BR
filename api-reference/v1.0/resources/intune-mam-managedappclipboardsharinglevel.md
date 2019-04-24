---
title: tipo de enumeração managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcbee5e0b7aa6343e31d57d14557bc0f0586fb80
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465199"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="19a03-103">tipo de enumeração managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="19a03-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="19a03-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19a03-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19a03-105">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="19a03-105">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="19a03-106">Membros</span><span class="sxs-lookup"><span data-stu-id="19a03-106">Members</span></span>
|<span data-ttu-id="19a03-107">Membro</span><span class="sxs-lookup"><span data-stu-id="19a03-107">Member</span></span>|<span data-ttu-id="19a03-108">Valor</span><span class="sxs-lookup"><span data-stu-id="19a03-108">Value</span></span>|<span data-ttu-id="19a03-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="19a03-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19a03-110">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="19a03-110">allApps</span></span>|<span data-ttu-id="19a03-111">,0</span><span class="sxs-lookup"><span data-stu-id="19a03-111">0</span></span>|<span data-ttu-id="19a03-112">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="19a03-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="19a03-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="19a03-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="19a03-114">1</span><span class="sxs-lookup"><span data-stu-id="19a03-114">1</span></span>|<span data-ttu-id="19a03-115">O compartilhamento é permitido entre todos os aplicativos gerenciados com colar ativado</span><span class="sxs-lookup"><span data-stu-id="19a03-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="19a03-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="19a03-116">managedApps</span></span>|<span data-ttu-id="19a03-117">duas</span><span class="sxs-lookup"><span data-stu-id="19a03-117">2</span></span>|<span data-ttu-id="19a03-118">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="19a03-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="19a03-119">bloqueou</span><span class="sxs-lookup"><span data-stu-id="19a03-119">blocked</span></span>|<span data-ttu-id="19a03-120">3D</span><span class="sxs-lookup"><span data-stu-id="19a03-120">3</span></span>|<span data-ttu-id="19a03-121">O compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="19a03-121">Sharing between apps is disabled</span></span>|



