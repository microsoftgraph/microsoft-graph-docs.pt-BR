---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b339074d33a0d501de12e12fa2ea9b2682fb7fe6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795909"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="e1fd7-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="e1fd7-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="e1fd7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1fd7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1fd7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1fd7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1fd7-106">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="e1fd7-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="e1fd7-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e1fd7-107">Members</span></span>
|<span data-ttu-id="e1fd7-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e1fd7-108">Member</span></span>|<span data-ttu-id="e1fd7-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e1fd7-109">Value</span></span>|<span data-ttu-id="e1fd7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1fd7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1fd7-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e1fd7-111">notConfigured</span></span>|<span data-ttu-id="e1fd7-112">,0</span><span class="sxs-lookup"><span data-stu-id="e1fd7-112">0</span></span>|<span data-ttu-id="e1fd7-113">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="e1fd7-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="e1fd7-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="e1fd7-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="e1fd7-115">1</span><span class="sxs-lookup"><span data-stu-id="e1fd7-115">1</span></span>|<span data-ttu-id="e1fd7-116">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e1fd7-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="e1fd7-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="e1fd7-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="e1fd7-118">duas</span><span class="sxs-lookup"><span data-stu-id="e1fd7-118">2</span></span>|<span data-ttu-id="e1fd7-119">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e1fd7-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="e1fd7-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="e1fd7-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="e1fd7-121">3D</span><span class="sxs-lookup"><span data-stu-id="e1fd7-121">3</span></span>|<span data-ttu-id="e1fd7-122">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="e1fd7-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="e1fd7-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="e1fd7-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="e1fd7-124">4 </span><span class="sxs-lookup"><span data-stu-id="e1fd7-124">4</span></span>|<span data-ttu-id="e1fd7-125">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="e1fd7-125">Audit Windows components, store apps and smart locker.</span></span>|



