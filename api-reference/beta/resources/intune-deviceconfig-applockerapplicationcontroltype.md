---
title: tipo de enum appLockerApplicationControlType
description: Valores possíveis de tipos de controle do aplicativo de AppLocker
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9ca34a44b1ea4e55199eb65283f839cb50e222da
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807802"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="eb59d-103">tipo de enum appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="eb59d-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="eb59d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eb59d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb59d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eb59d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb59d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eb59d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb59d-107">Valores possíveis de tipos de controle do aplicativo de AppLocker</span><span class="sxs-lookup"><span data-stu-id="eb59d-107">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="eb59d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="eb59d-108">Members</span></span>
|<span data-ttu-id="eb59d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="eb59d-109">Member</span></span>|<span data-ttu-id="eb59d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="eb59d-110">Value</span></span>|<span data-ttu-id="eb59d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb59d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb59d-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="eb59d-112">notConfigured</span></span>|<span data-ttu-id="eb59d-113">0</span><span class="sxs-lookup"><span data-stu-id="eb59d-113">0</span></span>|<span data-ttu-id="eb59d-114">Valor de padrão de dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="eb59d-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="eb59d-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="eb59d-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="eb59d-116">1</span><span class="sxs-lookup"><span data-stu-id="eb59d-116">1</span></span>|<span data-ttu-id="eb59d-117">Impor o componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="eb59d-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="eb59d-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="eb59d-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="eb59d-119">2</span><span class="sxs-lookup"><span data-stu-id="eb59d-119">2</span></span>|<span data-ttu-id="eb59d-120">Auditoria do componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="eb59d-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="eb59d-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="eb59d-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="eb59d-122">3</span><span class="sxs-lookup"><span data-stu-id="eb59d-122">3</span></span>|<span data-ttu-id="eb59d-123">Aplicar os componentes do Windows, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="eb59d-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="eb59d-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="eb59d-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="eb59d-125">4</span><span class="sxs-lookup"><span data-stu-id="eb59d-125">4</span></span>|<span data-ttu-id="eb59d-126">Componentes do Windows de auditoria, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="eb59d-126">Audit Windows components, store apps and smart locker.</span></span>|





