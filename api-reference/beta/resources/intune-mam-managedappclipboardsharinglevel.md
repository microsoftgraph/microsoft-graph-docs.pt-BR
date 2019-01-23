---
title: tipo de enum managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ccd90e4d704a075eaf43650fa765fabf3ab0b99
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410984"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="85dfb-103">tipo de enum managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="85dfb-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="85dfb-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="85dfb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="85dfb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="85dfb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85dfb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="85dfb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85dfb-107">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="85dfb-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="85dfb-108">Membros</span><span class="sxs-lookup"><span data-stu-id="85dfb-108">Members</span></span>
|<span data-ttu-id="85dfb-109">Membro</span><span class="sxs-lookup"><span data-stu-id="85dfb-109">Member</span></span>|<span data-ttu-id="85dfb-110">Valor</span><span class="sxs-lookup"><span data-stu-id="85dfb-110">Value</span></span>|<span data-ttu-id="85dfb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="85dfb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85dfb-112">allApps</span><span class="sxs-lookup"><span data-stu-id="85dfb-112">allApps</span></span>|<span data-ttu-id="85dfb-113">0</span><span class="sxs-lookup"><span data-stu-id="85dfb-113">0</span></span>|<span data-ttu-id="85dfb-114">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="85dfb-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="85dfb-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="85dfb-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="85dfb-116">1</span><span class="sxs-lookup"><span data-stu-id="85dfb-116">1</span></span>|<span data-ttu-id="85dfb-117">O compartilhamento é permitido entre todos os aplicativos gerenciados com Colar no habilitado</span><span class="sxs-lookup"><span data-stu-id="85dfb-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="85dfb-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="85dfb-118">managedApps</span></span>|<span data-ttu-id="85dfb-119">2</span><span class="sxs-lookup"><span data-stu-id="85dfb-119">2</span></span>|<span data-ttu-id="85dfb-120">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="85dfb-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="85dfb-121">bloqueado</span><span class="sxs-lookup"><span data-stu-id="85dfb-121">blocked</span></span>|<span data-ttu-id="85dfb-122">3</span><span class="sxs-lookup"><span data-stu-id="85dfb-122">3</span></span>|<span data-ttu-id="85dfb-123">Compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="85dfb-123">Sharing between apps is disabled</span></span>|




