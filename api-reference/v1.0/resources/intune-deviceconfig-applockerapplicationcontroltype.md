---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b1e463959cf4b5b39076fcf200b1c61ea0e73c0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257075"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="1fc3f-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="1fc3f-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="1fc3f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1fc3f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fc3f-105">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="1fc3f-105">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="1fc3f-106">Membros</span><span class="sxs-lookup"><span data-stu-id="1fc3f-106">Members</span></span>
|<span data-ttu-id="1fc3f-107">Membro</span><span class="sxs-lookup"><span data-stu-id="1fc3f-107">Member</span></span>|<span data-ttu-id="1fc3f-108">Valor</span><span class="sxs-lookup"><span data-stu-id="1fc3f-108">Value</span></span>|<span data-ttu-id="1fc3f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fc3f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fc3f-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1fc3f-110">notConfigured</span></span>|<span data-ttu-id="1fc3f-111">,0</span><span class="sxs-lookup"><span data-stu-id="1fc3f-111">0</span></span>|<span data-ttu-id="1fc3f-112">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="1fc3f-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="1fc3f-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="1fc3f-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="1fc3f-114">1</span><span class="sxs-lookup"><span data-stu-id="1fc3f-114">1</span></span>|<span data-ttu-id="1fc3f-115">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="1fc3f-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="1fc3f-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="1fc3f-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="1fc3f-117">duas</span><span class="sxs-lookup"><span data-stu-id="1fc3f-117">2</span></span>|<span data-ttu-id="1fc3f-118">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="1fc3f-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="1fc3f-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="1fc3f-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="1fc3f-120">3D</span><span class="sxs-lookup"><span data-stu-id="1fc3f-120">3</span></span>|<span data-ttu-id="1fc3f-121">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="1fc3f-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="1fc3f-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="1fc3f-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="1fc3f-123">quatro</span><span class="sxs-lookup"><span data-stu-id="1fc3f-123">4</span></span>|<span data-ttu-id="1fc3f-124">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="1fc3f-124">Audit Windows components, store apps and smart locker.</span></span>|



