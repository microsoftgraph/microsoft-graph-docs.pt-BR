---
title: tipo de enum managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
ms.openlocfilehash: 71c4ab2d629fdfee3ded68612d7060a0fa069809
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040608"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="b6f98-103">tipo de enum managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="b6f98-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="b6f98-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b6f98-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6f98-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b6f98-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6f98-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b6f98-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6f98-107">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="b6f98-107">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="b6f98-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b6f98-108">Members</span></span>
|<span data-ttu-id="b6f98-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b6f98-109">Member</span></span>|<span data-ttu-id="b6f98-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b6f98-110">Value</span></span>|<span data-ttu-id="b6f98-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6f98-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6f98-112">allApps</span><span class="sxs-lookup"><span data-stu-id="b6f98-112">allApps</span></span>|<span data-ttu-id="b6f98-113">0</span><span class="sxs-lookup"><span data-stu-id="b6f98-113">0</span></span>|<span data-ttu-id="b6f98-114">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="b6f98-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="b6f98-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="b6f98-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="b6f98-116">1</span><span class="sxs-lookup"><span data-stu-id="b6f98-116">1</span></span>|<span data-ttu-id="b6f98-117">O compartilhamento é permitido entre todos os aplicativos gerenciados com Colar no habilitado</span><span class="sxs-lookup"><span data-stu-id="b6f98-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="b6f98-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="b6f98-118">managedApps</span></span>|<span data-ttu-id="b6f98-119">2</span><span class="sxs-lookup"><span data-stu-id="b6f98-119">2</span></span>|<span data-ttu-id="b6f98-120">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="b6f98-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="b6f98-121">bloqueado</span><span class="sxs-lookup"><span data-stu-id="b6f98-121">blocked</span></span>|<span data-ttu-id="b6f98-122">3</span><span class="sxs-lookup"><span data-stu-id="b6f98-122">3</span></span>|<span data-ttu-id="b6f98-123">Compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="b6f98-123">Sharing between apps is disabled</span></span>|





