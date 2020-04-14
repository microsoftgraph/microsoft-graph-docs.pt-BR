---
title: tipo de enumeração managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f854a18bfcfac3f937c976180bbc4a423abbae0d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43374034"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="4e93b-103">tipo de enumeração managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="4e93b-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="4e93b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e93b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e93b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e93b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e93b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e93b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e93b-107">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="4e93b-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="4e93b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4e93b-108">Members</span></span>
|<span data-ttu-id="4e93b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4e93b-109">Member</span></span>|<span data-ttu-id="4e93b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4e93b-110">Value</span></span>|<span data-ttu-id="4e93b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e93b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e93b-112">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="4e93b-112">allApps</span></span>|<span data-ttu-id="4e93b-113">,0</span><span class="sxs-lookup"><span data-stu-id="4e93b-113">0</span></span>|<span data-ttu-id="4e93b-114">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="4e93b-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="4e93b-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="4e93b-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="4e93b-116">1</span><span class="sxs-lookup"><span data-stu-id="4e93b-116">1</span></span>|<span data-ttu-id="4e93b-117">O compartilhamento é permitido entre todos os aplicativos gerenciados com colar ativado</span><span class="sxs-lookup"><span data-stu-id="4e93b-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="4e93b-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="4e93b-118">managedApps</span></span>|<span data-ttu-id="4e93b-119">duas</span><span class="sxs-lookup"><span data-stu-id="4e93b-119">2</span></span>|<span data-ttu-id="4e93b-120">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="4e93b-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="4e93b-121">bloqueou</span><span class="sxs-lookup"><span data-stu-id="4e93b-121">blocked</span></span>|<span data-ttu-id="4e93b-122">3D</span><span class="sxs-lookup"><span data-stu-id="4e93b-122">3</span></span>|<span data-ttu-id="4e93b-123">O compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="4e93b-123">Sharing between apps is disabled</span></span>|



