---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9b4a20a79454f1aba1f162812a7fc4d7a324c359
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028564"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="0c3b8-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="0c3b8-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="0c3b8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c3b8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c3b8-105">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="0c3b8-105">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="0c3b8-106">Membros</span><span class="sxs-lookup"><span data-stu-id="0c3b8-106">Members</span></span>
|<span data-ttu-id="0c3b8-107">Membro</span><span class="sxs-lookup"><span data-stu-id="0c3b8-107">Member</span></span>|<span data-ttu-id="0c3b8-108">Valor</span><span class="sxs-lookup"><span data-stu-id="0c3b8-108">Value</span></span>|<span data-ttu-id="0c3b8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c3b8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c3b8-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0c3b8-110">notConfigured</span></span>|<span data-ttu-id="0c3b8-111">,0</span><span class="sxs-lookup"><span data-stu-id="0c3b8-111">0</span></span>|<span data-ttu-id="0c3b8-112">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="0c3b8-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="0c3b8-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0c3b8-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="0c3b8-114">1</span><span class="sxs-lookup"><span data-stu-id="0c3b8-114">1</span></span>|<span data-ttu-id="0c3b8-115">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="0c3b8-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="0c3b8-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0c3b8-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="0c3b8-117">duas</span><span class="sxs-lookup"><span data-stu-id="0c3b8-117">2</span></span>|<span data-ttu-id="0c3b8-118">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="0c3b8-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="0c3b8-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0c3b8-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0c3b8-120">3D</span><span class="sxs-lookup"><span data-stu-id="0c3b8-120">3</span></span>|<span data-ttu-id="0c3b8-121">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="0c3b8-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="0c3b8-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0c3b8-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0c3b8-123">quatro</span><span class="sxs-lookup"><span data-stu-id="0c3b8-123">4</span></span>|<span data-ttu-id="0c3b8-124">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="0c3b8-124">Audit Windows components, store apps and smart locker.</span></span>|



