---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: efdb7913d5b813ec528969520e2e7d64da1d3002
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708813"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="93131-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="93131-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="93131-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93131-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93131-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93131-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93131-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93131-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93131-107">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="93131-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="93131-108">Membros</span><span class="sxs-lookup"><span data-stu-id="93131-108">Members</span></span>
|<span data-ttu-id="93131-109">Membro</span><span class="sxs-lookup"><span data-stu-id="93131-109">Member</span></span>|<span data-ttu-id="93131-110">Valor</span><span class="sxs-lookup"><span data-stu-id="93131-110">Value</span></span>|<span data-ttu-id="93131-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="93131-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93131-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="93131-112">notConfigured</span></span>|<span data-ttu-id="93131-113">,0</span><span class="sxs-lookup"><span data-stu-id="93131-113">0</span></span>|<span data-ttu-id="93131-114">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="93131-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="93131-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="93131-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="93131-116">1</span><span class="sxs-lookup"><span data-stu-id="93131-116">1</span></span>|<span data-ttu-id="93131-117">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="93131-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="93131-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="93131-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="93131-119">duas</span><span class="sxs-lookup"><span data-stu-id="93131-119">2</span></span>|<span data-ttu-id="93131-120">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="93131-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="93131-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="93131-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="93131-122">3D</span><span class="sxs-lookup"><span data-stu-id="93131-122">3</span></span>|<span data-ttu-id="93131-123">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="93131-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="93131-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="93131-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="93131-125">4 </span><span class="sxs-lookup"><span data-stu-id="93131-125">4</span></span>|<span data-ttu-id="93131-126">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="93131-126">Audit Windows components, store apps and smart locker.</span></span>|





