---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dba073db7bf9cfb948fa5f3c76ce4294f1ee51f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333888"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="79211-103">tipo de enumeração appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="79211-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="79211-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79211-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79211-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79211-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79211-106">Valores possíveis dos tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="79211-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="79211-107">Membros</span><span class="sxs-lookup"><span data-stu-id="79211-107">Members</span></span>
|<span data-ttu-id="79211-108">Membro</span><span class="sxs-lookup"><span data-stu-id="79211-108">Member</span></span>|<span data-ttu-id="79211-109">Valor</span><span class="sxs-lookup"><span data-stu-id="79211-109">Value</span></span>|<span data-ttu-id="79211-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="79211-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79211-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="79211-111">notConfigured</span></span>|<span data-ttu-id="79211-112">,0</span><span class="sxs-lookup"><span data-stu-id="79211-112">0</span></span>|<span data-ttu-id="79211-113">Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="79211-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="79211-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="79211-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="79211-115">1</span><span class="sxs-lookup"><span data-stu-id="79211-115">1</span></span>|<span data-ttu-id="79211-116">Aplicar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="79211-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="79211-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="79211-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="79211-118">duas</span><span class="sxs-lookup"><span data-stu-id="79211-118">2</span></span>|<span data-ttu-id="79211-119">Auditar o componente do Windows e armazenar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="79211-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="79211-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="79211-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="79211-121">3D</span><span class="sxs-lookup"><span data-stu-id="79211-121">3</span></span>|<span data-ttu-id="79211-122">Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="79211-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="79211-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="79211-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="79211-124">quatro</span><span class="sxs-lookup"><span data-stu-id="79211-124">4</span></span>|<span data-ttu-id="79211-125">Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.</span><span class="sxs-lookup"><span data-stu-id="79211-125">Audit Windows components, store apps and smart locker.</span></span>|



