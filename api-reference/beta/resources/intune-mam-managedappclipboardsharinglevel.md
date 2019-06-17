---
title: tipo de enumeração managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7c03aeffe8e83a51caadba952e09af1fce06593
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991978"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="55f25-103">tipo de enumeração managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="55f25-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="55f25-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55f25-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55f25-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55f25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55f25-106">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="55f25-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="55f25-107">Membros</span><span class="sxs-lookup"><span data-stu-id="55f25-107">Members</span></span>
|<span data-ttu-id="55f25-108">Membro</span><span class="sxs-lookup"><span data-stu-id="55f25-108">Member</span></span>|<span data-ttu-id="55f25-109">Valor</span><span class="sxs-lookup"><span data-stu-id="55f25-109">Value</span></span>|<span data-ttu-id="55f25-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="55f25-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55f25-111">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="55f25-111">allApps</span></span>|<span data-ttu-id="55f25-112">,0</span><span class="sxs-lookup"><span data-stu-id="55f25-112">0</span></span>|<span data-ttu-id="55f25-113">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="55f25-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="55f25-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="55f25-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="55f25-115">1</span><span class="sxs-lookup"><span data-stu-id="55f25-115">1</span></span>|<span data-ttu-id="55f25-116">O compartilhamento é permitido entre todos os aplicativos gerenciados com colar ativado</span><span class="sxs-lookup"><span data-stu-id="55f25-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="55f25-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="55f25-117">managedApps</span></span>|<span data-ttu-id="55f25-118">duas</span><span class="sxs-lookup"><span data-stu-id="55f25-118">2</span></span>|<span data-ttu-id="55f25-119">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="55f25-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="55f25-120">bloqueou</span><span class="sxs-lookup"><span data-stu-id="55f25-120">blocked</span></span>|<span data-ttu-id="55f25-121">3D</span><span class="sxs-lookup"><span data-stu-id="55f25-121">3</span></span>|<span data-ttu-id="55f25-122">O compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="55f25-122">Sharing between apps is disabled</span></span>|





