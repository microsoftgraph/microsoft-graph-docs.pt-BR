---
title: tipo de enumeração managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8372d7a959a54a91d13aec91d2b27829fcf3a30c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074969"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="fcd48-103">tipo de enumeração managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="fcd48-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="fcd48-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcd48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcd48-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fcd48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcd48-106">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="fcd48-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="fcd48-107">Membros</span><span class="sxs-lookup"><span data-stu-id="fcd48-107">Members</span></span>
|<span data-ttu-id="fcd48-108">Membro</span><span class="sxs-lookup"><span data-stu-id="fcd48-108">Member</span></span>|<span data-ttu-id="fcd48-109">Valor</span><span class="sxs-lookup"><span data-stu-id="fcd48-109">Value</span></span>|<span data-ttu-id="fcd48-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcd48-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcd48-111">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="fcd48-111">allApps</span></span>|<span data-ttu-id="fcd48-112">,0</span><span class="sxs-lookup"><span data-stu-id="fcd48-112">0</span></span>|<span data-ttu-id="fcd48-113">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="fcd48-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="fcd48-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="fcd48-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="fcd48-115">1 </span><span class="sxs-lookup"><span data-stu-id="fcd48-115">1</span></span>|<span data-ttu-id="fcd48-116">O compartilhamento é permitido entre todos os aplicativos gerenciados com colar ativado</span><span class="sxs-lookup"><span data-stu-id="fcd48-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="fcd48-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="fcd48-117">managedApps</span></span>|<span data-ttu-id="fcd48-118">2 </span><span class="sxs-lookup"><span data-stu-id="fcd48-118">2</span></span>|<span data-ttu-id="fcd48-119">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="fcd48-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="fcd48-120">bloqueou</span><span class="sxs-lookup"><span data-stu-id="fcd48-120">blocked</span></span>|<span data-ttu-id="fcd48-121">3D</span><span class="sxs-lookup"><span data-stu-id="fcd48-121">3</span></span>|<span data-ttu-id="fcd48-122">O compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="fcd48-122">Sharing between apps is disabled</span></span>|









