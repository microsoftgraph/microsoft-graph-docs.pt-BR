---
title: tipo de enum appLockerApplicationControlType
description: Valores possíveis de tipos de controle do aplicativo de AppLocker
author: tfitzmac
ms.openlocfilehash: d53c2d0f7996edfab610e4206f4d2815ba4000b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310259"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="e0a6a-103">tipo de enum appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="e0a6a-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="e0a6a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e0a6a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0a6a-105">Valores possíveis de tipos de controle do aplicativo de AppLocker</span><span class="sxs-lookup"><span data-stu-id="e0a6a-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="e0a6a-106">Membros</span><span class="sxs-lookup"><span data-stu-id="e0a6a-106">Members</span></span>
|<span data-ttu-id="e0a6a-107">Membro</span><span class="sxs-lookup"><span data-stu-id="e0a6a-107">Member</span></span>|<span data-ttu-id="e0a6a-108">Valor</span><span class="sxs-lookup"><span data-stu-id="e0a6a-108">Value</span></span>|<span data-ttu-id="e0a6a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0a6a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0a6a-110">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="e0a6a-110">notConfigured</span></span>|<span data-ttu-id="e0a6a-111">0</span><span class="sxs-lookup"><span data-stu-id="e0a6a-111">0</span></span>|<span data-ttu-id="e0a6a-112">Valor de padrão de dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="e0a6a-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="e0a6a-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="e0a6a-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="e0a6a-114">1</span><span class="sxs-lookup"><span data-stu-id="e0a6a-114">1</span></span>|<span data-ttu-id="e0a6a-115">Impor o componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="e0a6a-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="e0a6a-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="e0a6a-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="e0a6a-117">2</span><span class="sxs-lookup"><span data-stu-id="e0a6a-117">2</span></span>|<span data-ttu-id="e0a6a-118">Auditoria do componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="e0a6a-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="e0a6a-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="e0a6a-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="e0a6a-120">3</span><span class="sxs-lookup"><span data-stu-id="e0a6a-120">3</span></span>|<span data-ttu-id="e0a6a-121">Aplicar os componentes do Windows, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e0a6a-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="e0a6a-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="e0a6a-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="e0a6a-123">4</span><span class="sxs-lookup"><span data-stu-id="e0a6a-123">4</span></span>|<span data-ttu-id="e0a6a-124">Componentes do Windows de auditoria, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e0a6a-124">Audit Windows components, store apps and smart locker.</span></span>|



