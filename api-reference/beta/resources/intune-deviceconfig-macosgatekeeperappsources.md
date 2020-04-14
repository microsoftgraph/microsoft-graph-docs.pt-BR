---
title: tipo de enumeração macOSGatekeeperAppSources
description: Opções de origem do aplicativo para gatekeeper do macOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 53e98d727f2c90d830b66106d3376564e6c89116
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464132"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="19162-103">tipo de enumeração macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="19162-103">macOSGatekeeperAppSources enum type</span></span>

<span data-ttu-id="19162-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19162-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19162-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="19162-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19162-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19162-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19162-107">Opções de origem do aplicativo para gatekeeper do macOS.</span><span class="sxs-lookup"><span data-stu-id="19162-107">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="19162-108">Membros</span><span class="sxs-lookup"><span data-stu-id="19162-108">Members</span></span>
|<span data-ttu-id="19162-109">Membro</span><span class="sxs-lookup"><span data-stu-id="19162-109">Member</span></span>|<span data-ttu-id="19162-110">Valor</span><span class="sxs-lookup"><span data-stu-id="19162-110">Value</span></span>|<span data-ttu-id="19162-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="19162-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19162-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="19162-112">notConfigured</span></span>|<span data-ttu-id="19162-113">,0</span><span class="sxs-lookup"><span data-stu-id="19162-113">0</span></span>|<span data-ttu-id="19162-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="19162-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="19162-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="19162-115">macAppStore</span></span>|<span data-ttu-id="19162-116">1</span><span class="sxs-lookup"><span data-stu-id="19162-116">1</span></span>|<span data-ttu-id="19162-117">Somente aplicativos do Mac loja podem ser executados.</span><span class="sxs-lookup"><span data-stu-id="19162-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="19162-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="19162-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="19162-119">duas</span><span class="sxs-lookup"><span data-stu-id="19162-119">2</span></span>|<span data-ttu-id="19162-120">Somente os aplicativos do Mac loja e dos desenvolvedores identificados podem ser executados.</span><span class="sxs-lookup"><span data-stu-id="19162-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="19162-121">em qualquer lugar</span><span class="sxs-lookup"><span data-stu-id="19162-121">anywhere</span></span>|<span data-ttu-id="19162-122">3D</span><span class="sxs-lookup"><span data-stu-id="19162-122">3</span></span>|<span data-ttu-id="19162-123">Os aplicativos de qualquer lugar podem ser executados.</span><span class="sxs-lookup"><span data-stu-id="19162-123">Apps from anywhere can be run.</span></span>|



