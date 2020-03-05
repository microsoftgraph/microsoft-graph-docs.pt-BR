---
title: tipo de enumeração iosKioskModeAppType
description: Opções de origem do aplicativo para o modo quiosque do iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 03e5d1c20f64a816160e2d9fa4292388d49bb50b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529889"
---
# <a name="ioskioskmodeapptype-enum-type"></a><span data-ttu-id="68441-103">tipo de enumeração iosKioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="68441-103">iosKioskModeAppType enum type</span></span>

<span data-ttu-id="68441-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="68441-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68441-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="68441-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68441-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68441-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68441-107">Opções de origem do aplicativo para o modo quiosque do iOS.</span><span class="sxs-lookup"><span data-stu-id="68441-107">App source options for iOS kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="68441-108">Membros</span><span class="sxs-lookup"><span data-stu-id="68441-108">Members</span></span>
|<span data-ttu-id="68441-109">Membro</span><span class="sxs-lookup"><span data-stu-id="68441-109">Member</span></span>|<span data-ttu-id="68441-110">Valor</span><span class="sxs-lookup"><span data-stu-id="68441-110">Value</span></span>|<span data-ttu-id="68441-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="68441-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68441-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="68441-112">notConfigured</span></span>|<span data-ttu-id="68441-113">,0</span><span class="sxs-lookup"><span data-stu-id="68441-113">0</span></span>|<span data-ttu-id="68441-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="68441-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="68441-115">appStoreApp</span><span class="sxs-lookup"><span data-stu-id="68441-115">appStoreApp</span></span>|<span data-ttu-id="68441-116">1 </span><span class="sxs-lookup"><span data-stu-id="68441-116">1</span></span>|<span data-ttu-id="68441-117">O aplicativo a ser executado vem da loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="68441-117">The app to be run comes from the app store.</span></span>|
|<span data-ttu-id="68441-118">managedApp</span><span class="sxs-lookup"><span data-stu-id="68441-118">managedApp</span></span>|<span data-ttu-id="68441-119">2 </span><span class="sxs-lookup"><span data-stu-id="68441-119">2</span></span>|<span data-ttu-id="68441-120">O aplicativo a ser executado está incorporado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="68441-120">The app to be run is built into the device.</span></span>|
|<span data-ttu-id="68441-121">builtInApp</span><span class="sxs-lookup"><span data-stu-id="68441-121">builtInApp</span></span>|<span data-ttu-id="68441-122">3 </span><span class="sxs-lookup"><span data-stu-id="68441-122">3</span></span>|<span data-ttu-id="68441-123">O aplicativo a ser executado é um aplicativo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="68441-123">The app to be run is a managed app.</span></span>|



