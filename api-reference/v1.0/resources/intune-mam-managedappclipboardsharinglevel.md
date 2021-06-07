---
title: Tipo de número managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 28a5d906342cc240d2382ed18c6de572e316f886
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754501"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="d525c-103">Tipo de número managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="d525c-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="d525c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d525c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d525c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d525c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d525c-106">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="d525c-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="d525c-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d525c-107">Members</span></span>
|<span data-ttu-id="d525c-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d525c-108">Member</span></span>|<span data-ttu-id="d525c-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d525c-109">Value</span></span>|<span data-ttu-id="d525c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d525c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d525c-111">allApps</span><span class="sxs-lookup"><span data-stu-id="d525c-111">allApps</span></span>|<span data-ttu-id="d525c-112">0</span><span class="sxs-lookup"><span data-stu-id="d525c-112">0</span></span>|<span data-ttu-id="d525c-113">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="d525c-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="d525c-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="d525c-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="d525c-115">1</span><span class="sxs-lookup"><span data-stu-id="d525c-115">1</span></span>|<span data-ttu-id="d525c-116">O compartilhamento é permitido entre todos os aplicativos gerenciados com a pasta habilitada</span><span class="sxs-lookup"><span data-stu-id="d525c-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="d525c-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="d525c-117">managedApps</span></span>|<span data-ttu-id="d525c-118">2</span><span class="sxs-lookup"><span data-stu-id="d525c-118">2</span></span>|<span data-ttu-id="d525c-119">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="d525c-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="d525c-120">blocked</span><span class="sxs-lookup"><span data-stu-id="d525c-120">blocked</span></span>|<span data-ttu-id="d525c-121">3</span><span class="sxs-lookup"><span data-stu-id="d525c-121">3</span></span>|<span data-ttu-id="d525c-122">O compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="d525c-122">Sharing between apps is disabled</span></span>|




