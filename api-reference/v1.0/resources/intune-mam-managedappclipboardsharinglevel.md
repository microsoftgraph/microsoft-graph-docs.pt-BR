---
title: tipo de enum managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
localization_priority: Normal
ms.openlocfilehash: 16d6e9154b3d6e683d9ddce0efd70a40c01c8994
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814312"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="90f3e-103">tipo de enum managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="90f3e-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="90f3e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="90f3e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90f3e-105">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="90f3e-105">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="90f3e-106">Membros</span><span class="sxs-lookup"><span data-stu-id="90f3e-106">Members</span></span>
|<span data-ttu-id="90f3e-107">Membro</span><span class="sxs-lookup"><span data-stu-id="90f3e-107">Member</span></span>|<span data-ttu-id="90f3e-108">Valor</span><span class="sxs-lookup"><span data-stu-id="90f3e-108">Value</span></span>|<span data-ttu-id="90f3e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="90f3e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90f3e-110">allApps</span><span class="sxs-lookup"><span data-stu-id="90f3e-110">allApps</span></span>|<span data-ttu-id="90f3e-111">0</span><span class="sxs-lookup"><span data-stu-id="90f3e-111">0</span></span>|<span data-ttu-id="90f3e-112">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="90f3e-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="90f3e-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="90f3e-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="90f3e-114">1</span><span class="sxs-lookup"><span data-stu-id="90f3e-114">1</span></span>|<span data-ttu-id="90f3e-115">O compartilhamento é permitido entre todos os aplicativos gerenciados com Colar no habilitado</span><span class="sxs-lookup"><span data-stu-id="90f3e-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="90f3e-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="90f3e-116">managedApps</span></span>|<span data-ttu-id="90f3e-117">2</span><span class="sxs-lookup"><span data-stu-id="90f3e-117">2</span></span>|<span data-ttu-id="90f3e-118">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="90f3e-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="90f3e-119">bloqueado</span><span class="sxs-lookup"><span data-stu-id="90f3e-119">blocked</span></span>|<span data-ttu-id="90f3e-120">3</span><span class="sxs-lookup"><span data-stu-id="90f3e-120">3</span></span>|<span data-ttu-id="90f3e-121">Compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="90f3e-121">Sharing between apps is disabled</span></span>|



