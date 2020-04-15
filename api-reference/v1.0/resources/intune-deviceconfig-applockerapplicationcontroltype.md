---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a0f2509aff44de9ebd2c4ae5ea7db63bccfa604f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449137"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="3fab7-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="3fab7-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="3fab7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fab7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3fab7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3fab7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fab7-106">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="3fab7-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="3fab7-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3fab7-107">Members</span></span>
|<span data-ttu-id="3fab7-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3fab7-108">Member</span></span>|<span data-ttu-id="3fab7-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3fab7-109">Value</span></span>|<span data-ttu-id="3fab7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fab7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fab7-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3fab7-111">notConfigured</span></span>|<span data-ttu-id="3fab7-112">,0</span><span class="sxs-lookup"><span data-stu-id="3fab7-112">0</span></span>|<span data-ttu-id="3fab7-113">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="3fab7-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="3fab7-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="3fab7-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="3fab7-115">1</span><span class="sxs-lookup"><span data-stu-id="3fab7-115">1</span></span>|<span data-ttu-id="3fab7-116">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="3fab7-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="3fab7-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="3fab7-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="3fab7-118">duas</span><span class="sxs-lookup"><span data-stu-id="3fab7-118">2</span></span>|<span data-ttu-id="3fab7-119">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="3fab7-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="3fab7-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="3fab7-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="3fab7-121">3D</span><span class="sxs-lookup"><span data-stu-id="3fab7-121">3</span></span>|<span data-ttu-id="3fab7-122">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="3fab7-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="3fab7-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="3fab7-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="3fab7-124">4 </span><span class="sxs-lookup"><span data-stu-id="3fab7-124">4</span></span>|<span data-ttu-id="3fab7-125">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="3fab7-125">Audit Windows components, store apps and smart locker.</span></span>|







