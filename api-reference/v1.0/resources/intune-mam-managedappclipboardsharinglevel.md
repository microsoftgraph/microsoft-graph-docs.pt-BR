---
title: tipo de enum managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
ms.openlocfilehash: 7cf7b4a2f6ea6dc129a21167a2d75ba215ff29fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007457"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="6de5f-103">tipo de enum managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="6de5f-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="6de5f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6de5f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6de5f-105">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="6de5f-105">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="6de5f-106">Membros</span><span class="sxs-lookup"><span data-stu-id="6de5f-106">Members</span></span>
|<span data-ttu-id="6de5f-107">Membro</span><span class="sxs-lookup"><span data-stu-id="6de5f-107">Member</span></span>|<span data-ttu-id="6de5f-108">Valor</span><span class="sxs-lookup"><span data-stu-id="6de5f-108">Value</span></span>|<span data-ttu-id="6de5f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6de5f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6de5f-110">allApps</span><span class="sxs-lookup"><span data-stu-id="6de5f-110">allApps</span></span>|<span data-ttu-id="6de5f-111">0</span><span class="sxs-lookup"><span data-stu-id="6de5f-111">0</span></span>|<span data-ttu-id="6de5f-112">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="6de5f-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="6de5f-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="6de5f-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="6de5f-114">1</span><span class="sxs-lookup"><span data-stu-id="6de5f-114">1</span></span>|<span data-ttu-id="6de5f-115">O compartilhamento é permitido entre todos os aplicativos gerenciados com Colar no habilitado</span><span class="sxs-lookup"><span data-stu-id="6de5f-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="6de5f-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="6de5f-116">managedApps</span></span>|<span data-ttu-id="6de5f-117">2</span><span class="sxs-lookup"><span data-stu-id="6de5f-117">2</span></span>|<span data-ttu-id="6de5f-118">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="6de5f-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="6de5f-119">bloqueado</span><span class="sxs-lookup"><span data-stu-id="6de5f-119">blocked</span></span>|<span data-ttu-id="6de5f-120">3</span><span class="sxs-lookup"><span data-stu-id="6de5f-120">3</span></span>|<span data-ttu-id="6de5f-121">Compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="6de5f-121">Sharing between apps is disabled</span></span>|



