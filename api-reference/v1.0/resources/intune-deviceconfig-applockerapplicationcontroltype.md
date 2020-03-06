---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ca428eb0ccf9121cc3a7b02e6abb333e0b4e5503
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530921"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="f4b76-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="f4b76-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="f4b76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4b76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4b76-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4b76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4b76-106">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="f4b76-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="f4b76-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f4b76-107">Members</span></span>
|<span data-ttu-id="f4b76-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f4b76-108">Member</span></span>|<span data-ttu-id="f4b76-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f4b76-109">Value</span></span>|<span data-ttu-id="f4b76-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4b76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4b76-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f4b76-111">notConfigured</span></span>|<span data-ttu-id="f4b76-112">,0</span><span class="sxs-lookup"><span data-stu-id="f4b76-112">0</span></span>|<span data-ttu-id="f4b76-113">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="f4b76-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="f4b76-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="f4b76-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="f4b76-115">1 </span><span class="sxs-lookup"><span data-stu-id="f4b76-115">1</span></span>|<span data-ttu-id="f4b76-116">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="f4b76-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="f4b76-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="f4b76-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="f4b76-118">2 </span><span class="sxs-lookup"><span data-stu-id="f4b76-118">2</span></span>|<span data-ttu-id="f4b76-119">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="f4b76-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="f4b76-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="f4b76-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="f4b76-121">3 </span><span class="sxs-lookup"><span data-stu-id="f4b76-121">3</span></span>|<span data-ttu-id="f4b76-122">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="f4b76-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="f4b76-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="f4b76-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="f4b76-124">4 </span><span class="sxs-lookup"><span data-stu-id="f4b76-124">4</span></span>|<span data-ttu-id="f4b76-125">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="f4b76-125">Audit Windows components, store apps and smart locker.</span></span>|




