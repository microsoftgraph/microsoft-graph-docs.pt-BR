---
title: tipo de enumeração managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 29c5fee1a6873e331a9adc927f1a92cf60a8c9e8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267072"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="495a2-103">tipo de enumeração managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="495a2-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="495a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="495a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="495a2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="495a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="495a2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="495a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="495a2-107">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="495a2-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="495a2-108">Membros</span><span class="sxs-lookup"><span data-stu-id="495a2-108">Members</span></span>
|<span data-ttu-id="495a2-109">Membro</span><span class="sxs-lookup"><span data-stu-id="495a2-109">Member</span></span>|<span data-ttu-id="495a2-110">Valor</span><span class="sxs-lookup"><span data-stu-id="495a2-110">Value</span></span>|<span data-ttu-id="495a2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="495a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="495a2-112">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="495a2-112">allApps</span></span>|<span data-ttu-id="495a2-113">,0</span><span class="sxs-lookup"><span data-stu-id="495a2-113">0</span></span>|<span data-ttu-id="495a2-114">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="495a2-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="495a2-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="495a2-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="495a2-116">1</span><span class="sxs-lookup"><span data-stu-id="495a2-116">1</span></span>|<span data-ttu-id="495a2-117">O compartilhamento é permitido entre todos os aplicativos gerenciados com colar ativado</span><span class="sxs-lookup"><span data-stu-id="495a2-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="495a2-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="495a2-118">managedApps</span></span>|<span data-ttu-id="495a2-119">duas</span><span class="sxs-lookup"><span data-stu-id="495a2-119">2</span></span>|<span data-ttu-id="495a2-120">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="495a2-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="495a2-121">bloqueou</span><span class="sxs-lookup"><span data-stu-id="495a2-121">blocked</span></span>|<span data-ttu-id="495a2-122">3D</span><span class="sxs-lookup"><span data-stu-id="495a2-122">3</span></span>|<span data-ttu-id="495a2-123">O compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="495a2-123">Sharing between apps is disabled</span></span>|




