---
title: tipo de enum appLockerApplicationControlType
description: Valores possíveis de tipos de controle do aplicativo de AppLocker
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 258a98b9ec4945c807a6aae2b34a178628952ac4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937954"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="56174-103">tipo de enum appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="56174-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="56174-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="56174-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56174-105">Valores possíveis de tipos de controle do aplicativo de AppLocker</span><span class="sxs-lookup"><span data-stu-id="56174-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="56174-106">Membros</span><span class="sxs-lookup"><span data-stu-id="56174-106">Members</span></span>
|<span data-ttu-id="56174-107">Membro</span><span class="sxs-lookup"><span data-stu-id="56174-107">Member</span></span>|<span data-ttu-id="56174-108">Valor</span><span class="sxs-lookup"><span data-stu-id="56174-108">Value</span></span>|<span data-ttu-id="56174-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="56174-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56174-110">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="56174-110">notConfigured</span></span>|<span data-ttu-id="56174-111">0</span><span class="sxs-lookup"><span data-stu-id="56174-111">0</span></span>|<span data-ttu-id="56174-112">Valor de padrão de dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="56174-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="56174-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="56174-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="56174-114">1</span><span class="sxs-lookup"><span data-stu-id="56174-114">1</span></span>|<span data-ttu-id="56174-115">Impor o componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="56174-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="56174-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="56174-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="56174-117">2</span><span class="sxs-lookup"><span data-stu-id="56174-117">2</span></span>|<span data-ttu-id="56174-118">Auditoria do componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="56174-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="56174-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="56174-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="56174-120">3</span><span class="sxs-lookup"><span data-stu-id="56174-120">3</span></span>|<span data-ttu-id="56174-121">Aplicar os componentes do Windows, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="56174-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="56174-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="56174-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="56174-123">4</span><span class="sxs-lookup"><span data-stu-id="56174-123">4</span></span>|<span data-ttu-id="56174-124">Componentes do Windows de auditoria, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="56174-124">Audit Windows components, store apps and smart locker.</span></span>|



