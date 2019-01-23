---
title: tipo de enum appLockerApplicationControlType
description: Valores possíveis de tipos de controle do aplicativo de AppLocker
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3bc89620a6dd13a65cfe40f37ba2f775e6a9c83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425719"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="86448-103">tipo de enum appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="86448-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="86448-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="86448-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="86448-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="86448-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86448-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="86448-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86448-107">Valores possíveis de tipos de controle do aplicativo de AppLocker</span><span class="sxs-lookup"><span data-stu-id="86448-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="86448-108">Membros</span><span class="sxs-lookup"><span data-stu-id="86448-108">Members</span></span>
|<span data-ttu-id="86448-109">Membro</span><span class="sxs-lookup"><span data-stu-id="86448-109">Member</span></span>|<span data-ttu-id="86448-110">Valor</span><span class="sxs-lookup"><span data-stu-id="86448-110">Value</span></span>|<span data-ttu-id="86448-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="86448-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86448-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="86448-112">notConfigured</span></span>|<span data-ttu-id="86448-113">0</span><span class="sxs-lookup"><span data-stu-id="86448-113">0</span></span>|<span data-ttu-id="86448-114">Valor de padrão de dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="86448-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="86448-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="86448-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="86448-116">1</span><span class="sxs-lookup"><span data-stu-id="86448-116">1</span></span>|<span data-ttu-id="86448-117">Impor o componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="86448-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="86448-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="86448-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="86448-119">2</span><span class="sxs-lookup"><span data-stu-id="86448-119">2</span></span>|<span data-ttu-id="86448-120">Auditoria do componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="86448-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="86448-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="86448-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="86448-122">3</span><span class="sxs-lookup"><span data-stu-id="86448-122">3</span></span>|<span data-ttu-id="86448-123">Aplicar os componentes do Windows, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="86448-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="86448-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="86448-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="86448-125">4</span><span class="sxs-lookup"><span data-stu-id="86448-125">4</span></span>|<span data-ttu-id="86448-126">Componentes do Windows de auditoria, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="86448-126">Audit Windows components, store apps and smart locker.</span></span>|




