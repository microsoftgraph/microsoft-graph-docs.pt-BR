---
title: tipo de enum managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 41983b9bb30880768fff0ee02883c32fcb5305a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968411"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="22db0-103">tipo de enum managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="22db0-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="22db0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="22db0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22db0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="22db0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22db0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="22db0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22db0-107">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="22db0-107">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="22db0-108">Membros</span><span class="sxs-lookup"><span data-stu-id="22db0-108">Members</span></span>
|<span data-ttu-id="22db0-109">Membro</span><span class="sxs-lookup"><span data-stu-id="22db0-109">Member</span></span>|<span data-ttu-id="22db0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="22db0-110">Value</span></span>|<span data-ttu-id="22db0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="22db0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22db0-112">allApps</span><span class="sxs-lookup"><span data-stu-id="22db0-112">allApps</span></span>|<span data-ttu-id="22db0-113">0</span><span class="sxs-lookup"><span data-stu-id="22db0-113">0</span></span>|<span data-ttu-id="22db0-114">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="22db0-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="22db0-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="22db0-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="22db0-116">1</span><span class="sxs-lookup"><span data-stu-id="22db0-116">1</span></span>|<span data-ttu-id="22db0-117">O compartilhamento é permitido entre todos os aplicativos gerenciados com Colar no habilitado</span><span class="sxs-lookup"><span data-stu-id="22db0-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="22db0-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="22db0-118">managedApps</span></span>|<span data-ttu-id="22db0-119">2</span><span class="sxs-lookup"><span data-stu-id="22db0-119">2</span></span>|<span data-ttu-id="22db0-120">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="22db0-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="22db0-121">bloqueado</span><span class="sxs-lookup"><span data-stu-id="22db0-121">blocked</span></span>|<span data-ttu-id="22db0-122">3</span><span class="sxs-lookup"><span data-stu-id="22db0-122">3</span></span>|<span data-ttu-id="22db0-123">Compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="22db0-123">Sharing between apps is disabled</span></span>|





