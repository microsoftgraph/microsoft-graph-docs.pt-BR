---
title: tipo de enumeração managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 97e5e74b9d8f039e75df61791ef8dea945e49818
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527962"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="4b766-103">tipo de enumeração managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="4b766-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="4b766-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4b766-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b766-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b766-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b766-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b766-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b766-107">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="4b766-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="4b766-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4b766-108">Members</span></span>
|<span data-ttu-id="4b766-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4b766-109">Member</span></span>|<span data-ttu-id="4b766-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4b766-110">Value</span></span>|<span data-ttu-id="4b766-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b766-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b766-112">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="4b766-112">allApps</span></span>|<span data-ttu-id="4b766-113">,0</span><span class="sxs-lookup"><span data-stu-id="4b766-113">0</span></span>|<span data-ttu-id="4b766-114">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="4b766-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="4b766-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="4b766-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="4b766-116">1 </span><span class="sxs-lookup"><span data-stu-id="4b766-116">1</span></span>|<span data-ttu-id="4b766-117">O compartilhamento é permitido entre todos os aplicativos gerenciados com colar ativado</span><span class="sxs-lookup"><span data-stu-id="4b766-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="4b766-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="4b766-118">managedApps</span></span>|<span data-ttu-id="4b766-119">2 </span><span class="sxs-lookup"><span data-stu-id="4b766-119">2</span></span>|<span data-ttu-id="4b766-120">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="4b766-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="4b766-121">bloqueou</span><span class="sxs-lookup"><span data-stu-id="4b766-121">blocked</span></span>|<span data-ttu-id="4b766-122">3 </span><span class="sxs-lookup"><span data-stu-id="4b766-122">3</span></span>|<span data-ttu-id="4b766-123">O compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="4b766-123">Sharing between apps is disabled</span></span>|



