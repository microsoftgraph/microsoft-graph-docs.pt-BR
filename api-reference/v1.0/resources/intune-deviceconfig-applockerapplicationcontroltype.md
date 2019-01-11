---
title: tipo de enum appLockerApplicationControlType
description: Valores possíveis de tipos de controle do aplicativo de AppLocker
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 241387f34a64b4b58d974fc21e2aa5d3af696736
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871978"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="ed308-103">tipo de enum appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="ed308-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="ed308-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ed308-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed308-105">Valores possíveis de tipos de controle do aplicativo de AppLocker</span><span class="sxs-lookup"><span data-stu-id="ed308-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="ed308-106">Membros</span><span class="sxs-lookup"><span data-stu-id="ed308-106">Members</span></span>
|<span data-ttu-id="ed308-107">Membro</span><span class="sxs-lookup"><span data-stu-id="ed308-107">Member</span></span>|<span data-ttu-id="ed308-108">Valor</span><span class="sxs-lookup"><span data-stu-id="ed308-108">Value</span></span>|<span data-ttu-id="ed308-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed308-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed308-110">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="ed308-110">notConfigured</span></span>|<span data-ttu-id="ed308-111">0</span><span class="sxs-lookup"><span data-stu-id="ed308-111">0</span></span>|<span data-ttu-id="ed308-112">Valor de padrão de dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="ed308-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="ed308-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="ed308-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="ed308-114">1</span><span class="sxs-lookup"><span data-stu-id="ed308-114">1</span></span>|<span data-ttu-id="ed308-115">Impor o componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="ed308-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="ed308-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="ed308-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="ed308-117">2</span><span class="sxs-lookup"><span data-stu-id="ed308-117">2</span></span>|<span data-ttu-id="ed308-118">Auditoria do componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="ed308-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="ed308-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="ed308-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="ed308-120">3</span><span class="sxs-lookup"><span data-stu-id="ed308-120">3</span></span>|<span data-ttu-id="ed308-121">Aplicar os componentes do Windows, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ed308-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="ed308-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="ed308-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="ed308-123">4</span><span class="sxs-lookup"><span data-stu-id="ed308-123">4</span></span>|<span data-ttu-id="ed308-124">Componentes do Windows de auditoria, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ed308-124">Audit Windows components, store apps and smart locker.</span></span>|



