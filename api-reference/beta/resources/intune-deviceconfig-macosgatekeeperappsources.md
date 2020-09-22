---
title: tipo de enumeração macOSGatekeeperAppSources
description: Opções de origem do aplicativo para gatekeeper do macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6a15faac35a273656d9fc03e10c1f73f0dced568
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024147"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="14154-103">tipo de enumeração macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="14154-103">macOSGatekeeperAppSources enum type</span></span>

<span data-ttu-id="14154-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14154-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14154-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14154-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14154-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14154-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14154-107">Opções de origem do aplicativo para gatekeeper do macOS.</span><span class="sxs-lookup"><span data-stu-id="14154-107">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="14154-108">Membros</span><span class="sxs-lookup"><span data-stu-id="14154-108">Members</span></span>
|<span data-ttu-id="14154-109">Membro</span><span class="sxs-lookup"><span data-stu-id="14154-109">Member</span></span>|<span data-ttu-id="14154-110">Valor</span><span class="sxs-lookup"><span data-stu-id="14154-110">Value</span></span>|<span data-ttu-id="14154-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="14154-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14154-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="14154-112">notConfigured</span></span>|<span data-ttu-id="14154-113">,0</span><span class="sxs-lookup"><span data-stu-id="14154-113">0</span></span>|<span data-ttu-id="14154-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="14154-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="14154-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="14154-115">macAppStore</span></span>|<span data-ttu-id="14154-116">1 </span><span class="sxs-lookup"><span data-stu-id="14154-116">1</span></span>|<span data-ttu-id="14154-117">Somente aplicativos do Mac loja podem ser executados.</span><span class="sxs-lookup"><span data-stu-id="14154-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="14154-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="14154-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="14154-119">2 </span><span class="sxs-lookup"><span data-stu-id="14154-119">2</span></span>|<span data-ttu-id="14154-120">Somente os aplicativos do Mac loja e dos desenvolvedores identificados podem ser executados.</span><span class="sxs-lookup"><span data-stu-id="14154-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="14154-121">em qualquer lugar</span><span class="sxs-lookup"><span data-stu-id="14154-121">anywhere</span></span>|<span data-ttu-id="14154-122">3 </span><span class="sxs-lookup"><span data-stu-id="14154-122">3</span></span>|<span data-ttu-id="14154-123">Os aplicativos de qualquer lugar podem ser executados.</span><span class="sxs-lookup"><span data-stu-id="14154-123">Apps from anywhere can be run.</span></span>|






