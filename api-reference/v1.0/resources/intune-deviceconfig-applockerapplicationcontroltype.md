---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b1e463959cf4b5b39076fcf200b1c61ea0e73c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575125"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="38815-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="38815-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="38815-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38815-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38815-105">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="38815-105">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="38815-106">Membros</span><span class="sxs-lookup"><span data-stu-id="38815-106">Members</span></span>
|<span data-ttu-id="38815-107">Membro</span><span class="sxs-lookup"><span data-stu-id="38815-107">Member</span></span>|<span data-ttu-id="38815-108">Valor</span><span class="sxs-lookup"><span data-stu-id="38815-108">Value</span></span>|<span data-ttu-id="38815-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="38815-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38815-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="38815-110">notConfigured</span></span>|<span data-ttu-id="38815-111">,0</span><span class="sxs-lookup"><span data-stu-id="38815-111">0</span></span>|<span data-ttu-id="38815-112">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="38815-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="38815-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="38815-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="38815-114">1 </span><span class="sxs-lookup"><span data-stu-id="38815-114">1</span></span>|<span data-ttu-id="38815-115">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="38815-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="38815-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="38815-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="38815-117">2 </span><span class="sxs-lookup"><span data-stu-id="38815-117">2</span></span>|<span data-ttu-id="38815-118">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="38815-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="38815-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="38815-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="38815-120">3 </span><span class="sxs-lookup"><span data-stu-id="38815-120">3</span></span>|<span data-ttu-id="38815-121">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="38815-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="38815-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="38815-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="38815-123">4 </span><span class="sxs-lookup"><span data-stu-id="38815-123">4</span></span>|<span data-ttu-id="38815-124">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="38815-124">Audit Windows components, store apps and smart locker.</span></span>|



