---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1b3e5ec545f4466eb080f20839e12c7e5972cc0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981577"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="18fbb-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="18fbb-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="18fbb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18fbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18fbb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18fbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18fbb-106">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="18fbb-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="18fbb-107">Membros</span><span class="sxs-lookup"><span data-stu-id="18fbb-107">Members</span></span>
|<span data-ttu-id="18fbb-108">Membro</span><span class="sxs-lookup"><span data-stu-id="18fbb-108">Member</span></span>|<span data-ttu-id="18fbb-109">Valor</span><span class="sxs-lookup"><span data-stu-id="18fbb-109">Value</span></span>|<span data-ttu-id="18fbb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="18fbb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18fbb-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="18fbb-111">notConfigured</span></span>|<span data-ttu-id="18fbb-112">,0</span><span class="sxs-lookup"><span data-stu-id="18fbb-112">0</span></span>|<span data-ttu-id="18fbb-113">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="18fbb-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="18fbb-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="18fbb-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="18fbb-115">1</span><span class="sxs-lookup"><span data-stu-id="18fbb-115">1</span></span>|<span data-ttu-id="18fbb-116">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="18fbb-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="18fbb-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="18fbb-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="18fbb-118">duas</span><span class="sxs-lookup"><span data-stu-id="18fbb-118">2</span></span>|<span data-ttu-id="18fbb-119">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="18fbb-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="18fbb-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="18fbb-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="18fbb-121">3D</span><span class="sxs-lookup"><span data-stu-id="18fbb-121">3</span></span>|<span data-ttu-id="18fbb-122">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="18fbb-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="18fbb-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="18fbb-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="18fbb-124">quatro</span><span class="sxs-lookup"><span data-stu-id="18fbb-124">4</span></span>|<span data-ttu-id="18fbb-125">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="18fbb-125">Audit Windows components, store apps and smart locker.</span></span>|





