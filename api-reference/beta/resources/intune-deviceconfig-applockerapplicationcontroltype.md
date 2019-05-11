---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7d40e76303389c95c6f68350b1c2bd1a03208d46
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947565"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="edaa3-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="edaa3-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="edaa3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="edaa3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edaa3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="edaa3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edaa3-106">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="edaa3-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="edaa3-107">Membros</span><span class="sxs-lookup"><span data-stu-id="edaa3-107">Members</span></span>
|<span data-ttu-id="edaa3-108">Membro</span><span class="sxs-lookup"><span data-stu-id="edaa3-108">Member</span></span>|<span data-ttu-id="edaa3-109">Valor</span><span class="sxs-lookup"><span data-stu-id="edaa3-109">Value</span></span>|<span data-ttu-id="edaa3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="edaa3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edaa3-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="edaa3-111">notConfigured</span></span>|<span data-ttu-id="edaa3-112">,0</span><span class="sxs-lookup"><span data-stu-id="edaa3-112">0</span></span>|<span data-ttu-id="edaa3-113">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="edaa3-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="edaa3-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="edaa3-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="edaa3-115">1</span><span class="sxs-lookup"><span data-stu-id="edaa3-115">1</span></span>|<span data-ttu-id="edaa3-116">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="edaa3-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="edaa3-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="edaa3-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="edaa3-118">duas</span><span class="sxs-lookup"><span data-stu-id="edaa3-118">2</span></span>|<span data-ttu-id="edaa3-119">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="edaa3-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="edaa3-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="edaa3-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="edaa3-121">3D</span><span class="sxs-lookup"><span data-stu-id="edaa3-121">3</span></span>|<span data-ttu-id="edaa3-122">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="edaa3-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="edaa3-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="edaa3-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="edaa3-124">quatro</span><span class="sxs-lookup"><span data-stu-id="edaa3-124">4</span></span>|<span data-ttu-id="edaa3-125">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="edaa3-125">Audit Windows components, store apps and smart locker.</span></span>|




