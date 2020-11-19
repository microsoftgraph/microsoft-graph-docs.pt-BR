---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8e645f0ee8201ee0e66fe21ce80cc237f52faa3a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260821"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="d562f-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="d562f-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="d562f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d562f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d562f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d562f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d562f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d562f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d562f-107">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="d562f-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="d562f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d562f-108">Members</span></span>
|<span data-ttu-id="d562f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d562f-109">Member</span></span>|<span data-ttu-id="d562f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d562f-110">Value</span></span>|<span data-ttu-id="d562f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d562f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d562f-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d562f-112">notConfigured</span></span>|<span data-ttu-id="d562f-113">,0</span><span class="sxs-lookup"><span data-stu-id="d562f-113">0</span></span>|<span data-ttu-id="d562f-114">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="d562f-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="d562f-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="d562f-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="d562f-116">1</span><span class="sxs-lookup"><span data-stu-id="d562f-116">1</span></span>|<span data-ttu-id="d562f-117">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d562f-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="d562f-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="d562f-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="d562f-119">duas</span><span class="sxs-lookup"><span data-stu-id="d562f-119">2</span></span>|<span data-ttu-id="d562f-120">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d562f-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="d562f-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="d562f-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="d562f-122">3D</span><span class="sxs-lookup"><span data-stu-id="d562f-122">3</span></span>|<span data-ttu-id="d562f-123">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="d562f-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="d562f-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="d562f-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="d562f-125">4 </span><span class="sxs-lookup"><span data-stu-id="d562f-125">4</span></span>|<span data-ttu-id="d562f-126">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="d562f-126">Audit Windows components, store apps and smart locker.</span></span>|




