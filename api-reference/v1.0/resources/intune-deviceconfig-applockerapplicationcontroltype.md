---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e34472e8f534f78167d57309bd7315102bf8a3b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051092"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="43b85-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="43b85-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="43b85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43b85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43b85-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43b85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43b85-106">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="43b85-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="43b85-107">Membros</span><span class="sxs-lookup"><span data-stu-id="43b85-107">Members</span></span>
|<span data-ttu-id="43b85-108">Membro</span><span class="sxs-lookup"><span data-stu-id="43b85-108">Member</span></span>|<span data-ttu-id="43b85-109">Valor</span><span class="sxs-lookup"><span data-stu-id="43b85-109">Value</span></span>|<span data-ttu-id="43b85-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="43b85-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43b85-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="43b85-111">notConfigured</span></span>|<span data-ttu-id="43b85-112">,0</span><span class="sxs-lookup"><span data-stu-id="43b85-112">0</span></span>|<span data-ttu-id="43b85-113">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="43b85-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="43b85-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="43b85-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="43b85-115">1 </span><span class="sxs-lookup"><span data-stu-id="43b85-115">1</span></span>|<span data-ttu-id="43b85-116">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="43b85-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="43b85-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="43b85-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="43b85-118">2 </span><span class="sxs-lookup"><span data-stu-id="43b85-118">2</span></span>|<span data-ttu-id="43b85-119">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="43b85-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="43b85-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="43b85-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="43b85-121">3 </span><span class="sxs-lookup"><span data-stu-id="43b85-121">3</span></span>|<span data-ttu-id="43b85-122">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="43b85-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="43b85-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="43b85-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="43b85-124">4 </span><span class="sxs-lookup"><span data-stu-id="43b85-124">4</span></span>|<span data-ttu-id="43b85-125">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="43b85-125">Audit Windows components, store apps and smart locker.</span></span>|









