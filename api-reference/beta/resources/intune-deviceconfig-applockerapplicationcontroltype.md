---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4fab692743e0e76b37e81ff88e7a4d464c96e17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549299"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="09ffe-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="09ffe-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="09ffe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09ffe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09ffe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09ffe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09ffe-106">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="09ffe-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="09ffe-107">Membros</span><span class="sxs-lookup"><span data-stu-id="09ffe-107">Members</span></span>
|<span data-ttu-id="09ffe-108">Membro</span><span class="sxs-lookup"><span data-stu-id="09ffe-108">Member</span></span>|<span data-ttu-id="09ffe-109">Valor</span><span class="sxs-lookup"><span data-stu-id="09ffe-109">Value</span></span>|<span data-ttu-id="09ffe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="09ffe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09ffe-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="09ffe-111">notConfigured</span></span>|<span data-ttu-id="09ffe-112">,0</span><span class="sxs-lookup"><span data-stu-id="09ffe-112">0</span></span>|<span data-ttu-id="09ffe-113">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="09ffe-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="09ffe-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="09ffe-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="09ffe-115">1 </span><span class="sxs-lookup"><span data-stu-id="09ffe-115">1</span></span>|<span data-ttu-id="09ffe-116">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="09ffe-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="09ffe-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="09ffe-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="09ffe-118">2 </span><span class="sxs-lookup"><span data-stu-id="09ffe-118">2</span></span>|<span data-ttu-id="09ffe-119">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="09ffe-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="09ffe-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="09ffe-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="09ffe-121">3 </span><span class="sxs-lookup"><span data-stu-id="09ffe-121">3</span></span>|<span data-ttu-id="09ffe-122">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="09ffe-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="09ffe-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="09ffe-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="09ffe-124">4 </span><span class="sxs-lookup"><span data-stu-id="09ffe-124">4</span></span>|<span data-ttu-id="09ffe-125">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="09ffe-125">Audit Windows components, store apps and smart locker.</span></span>|





