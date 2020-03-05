---
title: tipo de enumeração macOSGatekeeperAppSources
description: Opções de origem do aplicativo para gatekeeper do macOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7e0990d063d2f50045b3d5de7f4cce4f9f32943b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526108"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="775a0-103">tipo de enumeração macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="775a0-103">macOSGatekeeperAppSources enum type</span></span>

<span data-ttu-id="775a0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="775a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="775a0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="775a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="775a0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="775a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="775a0-107">Opções de origem do aplicativo para gatekeeper do macOS.</span><span class="sxs-lookup"><span data-stu-id="775a0-107">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="775a0-108">Membros</span><span class="sxs-lookup"><span data-stu-id="775a0-108">Members</span></span>
|<span data-ttu-id="775a0-109">Membro</span><span class="sxs-lookup"><span data-stu-id="775a0-109">Member</span></span>|<span data-ttu-id="775a0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="775a0-110">Value</span></span>|<span data-ttu-id="775a0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="775a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="775a0-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="775a0-112">notConfigured</span></span>|<span data-ttu-id="775a0-113">,0</span><span class="sxs-lookup"><span data-stu-id="775a0-113">0</span></span>|<span data-ttu-id="775a0-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="775a0-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="775a0-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="775a0-115">macAppStore</span></span>|<span data-ttu-id="775a0-116">1 </span><span class="sxs-lookup"><span data-stu-id="775a0-116">1</span></span>|<span data-ttu-id="775a0-117">Somente aplicativos do Mac loja podem ser executados.</span><span class="sxs-lookup"><span data-stu-id="775a0-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="775a0-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="775a0-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="775a0-119">2 </span><span class="sxs-lookup"><span data-stu-id="775a0-119">2</span></span>|<span data-ttu-id="775a0-120">Somente os aplicativos do Mac loja e dos desenvolvedores identificados podem ser executados.</span><span class="sxs-lookup"><span data-stu-id="775a0-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="775a0-121">em qualquer lugar</span><span class="sxs-lookup"><span data-stu-id="775a0-121">anywhere</span></span>|<span data-ttu-id="775a0-122">3 </span><span class="sxs-lookup"><span data-stu-id="775a0-122">3</span></span>|<span data-ttu-id="775a0-123">Os aplicativos de qualquer lugar podem ser executados.</span><span class="sxs-lookup"><span data-stu-id="775a0-123">Apps from anywhere can be run.</span></span>|



