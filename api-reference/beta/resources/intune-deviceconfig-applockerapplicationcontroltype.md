---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 07ce6969c79581ed33b3a34d75445f7bf5612598
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527076"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="f1ead-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="f1ead-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="f1ead-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f1ead-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1ead-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1ead-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1ead-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1ead-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1ead-107">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="f1ead-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="f1ead-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f1ead-108">Members</span></span>
|<span data-ttu-id="f1ead-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f1ead-109">Member</span></span>|<span data-ttu-id="f1ead-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f1ead-110">Value</span></span>|<span data-ttu-id="f1ead-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1ead-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1ead-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f1ead-112">notConfigured</span></span>|<span data-ttu-id="f1ead-113">,0</span><span class="sxs-lookup"><span data-stu-id="f1ead-113">0</span></span>|<span data-ttu-id="f1ead-114">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="f1ead-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="f1ead-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="f1ead-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="f1ead-116">1 </span><span class="sxs-lookup"><span data-stu-id="f1ead-116">1</span></span>|<span data-ttu-id="f1ead-117">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="f1ead-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="f1ead-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="f1ead-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="f1ead-119">2 </span><span class="sxs-lookup"><span data-stu-id="f1ead-119">2</span></span>|<span data-ttu-id="f1ead-120">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="f1ead-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="f1ead-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="f1ead-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="f1ead-122">3 </span><span class="sxs-lookup"><span data-stu-id="f1ead-122">3</span></span>|<span data-ttu-id="f1ead-123">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="f1ead-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="f1ead-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="f1ead-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="f1ead-125">4 </span><span class="sxs-lookup"><span data-stu-id="f1ead-125">4</span></span>|<span data-ttu-id="f1ead-126">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="f1ead-126">Audit Windows components, store apps and smart locker.</span></span>|



