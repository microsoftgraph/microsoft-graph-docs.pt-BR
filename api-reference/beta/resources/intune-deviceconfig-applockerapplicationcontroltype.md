---
title: tipo de enum appLockerApplicationControlType
description: Valores possíveis de tipos de controle do aplicativo de AppLocker
author: tfitzmac
ms.openlocfilehash: 0d6190170d6f6695a3303047f9ccb193afd248f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330202"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="04ad8-103">tipo de enum appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="04ad8-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="04ad8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="04ad8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04ad8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="04ad8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04ad8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="04ad8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04ad8-107">Valores possíveis de tipos de controle do aplicativo de AppLocker</span><span class="sxs-lookup"><span data-stu-id="04ad8-107">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="04ad8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="04ad8-108">Members</span></span>
|<span data-ttu-id="04ad8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="04ad8-109">Member</span></span>|<span data-ttu-id="04ad8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="04ad8-110">Value</span></span>|<span data-ttu-id="04ad8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="04ad8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04ad8-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="04ad8-112">notConfigured</span></span>|<span data-ttu-id="04ad8-113">0</span><span class="sxs-lookup"><span data-stu-id="04ad8-113">0</span></span>|<span data-ttu-id="04ad8-114">Valor de padrão de dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="04ad8-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="04ad8-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="04ad8-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="04ad8-116">1</span><span class="sxs-lookup"><span data-stu-id="04ad8-116">1</span></span>|<span data-ttu-id="04ad8-117">Impor o componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="04ad8-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="04ad8-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="04ad8-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="04ad8-119">2</span><span class="sxs-lookup"><span data-stu-id="04ad8-119">2</span></span>|<span data-ttu-id="04ad8-120">Auditoria do componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="04ad8-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="04ad8-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="04ad8-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="04ad8-122">3</span><span class="sxs-lookup"><span data-stu-id="04ad8-122">3</span></span>|<span data-ttu-id="04ad8-123">Aplicar os componentes do Windows, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="04ad8-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="04ad8-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="04ad8-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="04ad8-125">4</span><span class="sxs-lookup"><span data-stu-id="04ad8-125">4</span></span>|<span data-ttu-id="04ad8-126">Componentes do Windows de auditoria, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="04ad8-126">Audit Windows components, store apps and smart locker.</span></span>|





