---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4fab692743e0e76b37e81ff88e7a4d464c96e17
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799493"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="0e796-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="0e796-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="0e796-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e796-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e796-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e796-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e796-106">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="0e796-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="0e796-107">Membros</span><span class="sxs-lookup"><span data-stu-id="0e796-107">Members</span></span>
|<span data-ttu-id="0e796-108">Membro</span><span class="sxs-lookup"><span data-stu-id="0e796-108">Member</span></span>|<span data-ttu-id="0e796-109">Valor</span><span class="sxs-lookup"><span data-stu-id="0e796-109">Value</span></span>|<span data-ttu-id="0e796-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e796-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e796-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0e796-111">notConfigured</span></span>|<span data-ttu-id="0e796-112">,0</span><span class="sxs-lookup"><span data-stu-id="0e796-112">0</span></span>|<span data-ttu-id="0e796-113">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="0e796-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="0e796-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0e796-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="0e796-115">1</span><span class="sxs-lookup"><span data-stu-id="0e796-115">1</span></span>|<span data-ttu-id="0e796-116">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="0e796-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="0e796-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0e796-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="0e796-118">duas</span><span class="sxs-lookup"><span data-stu-id="0e796-118">2</span></span>|<span data-ttu-id="0e796-119">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="0e796-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="0e796-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0e796-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0e796-121">3D</span><span class="sxs-lookup"><span data-stu-id="0e796-121">3</span></span>|<span data-ttu-id="0e796-122">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="0e796-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="0e796-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0e796-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0e796-124">quatro</span><span class="sxs-lookup"><span data-stu-id="0e796-124">4</span></span>|<span data-ttu-id="0e796-125">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="0e796-125">Audit Windows components, store apps and smart locker.</span></span>|





