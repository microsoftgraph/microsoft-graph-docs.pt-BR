---
title: tipo de enum appLockerApplicationControlType
description: Valores possíveis de tipos de controle do aplicativo de AppLocker
ms.openlocfilehash: 703cc18dfee49a01adb3cd4f61c5d7e99e30fb00
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003976"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="f5804-103">tipo de enum appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="f5804-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="f5804-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f5804-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5804-105">Valores possíveis de tipos de controle do aplicativo de AppLocker</span><span class="sxs-lookup"><span data-stu-id="f5804-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="f5804-106">Membros</span><span class="sxs-lookup"><span data-stu-id="f5804-106">Members</span></span>
|<span data-ttu-id="f5804-107">Membro</span><span class="sxs-lookup"><span data-stu-id="f5804-107">Member</span></span>|<span data-ttu-id="f5804-108">Valor</span><span class="sxs-lookup"><span data-stu-id="f5804-108">Value</span></span>|<span data-ttu-id="f5804-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5804-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5804-110">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="f5804-110">notConfigured</span></span>|<span data-ttu-id="f5804-111">0</span><span class="sxs-lookup"><span data-stu-id="f5804-111">0</span></span>|<span data-ttu-id="f5804-112">Valor de padrão de dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="f5804-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="f5804-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="f5804-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="f5804-114">1</span><span class="sxs-lookup"><span data-stu-id="f5804-114">1</span></span>|<span data-ttu-id="f5804-115">Impor o componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="f5804-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="f5804-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="f5804-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="f5804-117">2</span><span class="sxs-lookup"><span data-stu-id="f5804-117">2</span></span>|<span data-ttu-id="f5804-118">Auditoria do componente e armazenamento de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="f5804-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="f5804-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="f5804-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="f5804-120">3</span><span class="sxs-lookup"><span data-stu-id="f5804-120">3</span></span>|<span data-ttu-id="f5804-121">Aplicar os componentes do Windows, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="f5804-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="f5804-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="f5804-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="f5804-123">4</span><span class="sxs-lookup"><span data-stu-id="f5804-123">4</span></span>|<span data-ttu-id="f5804-124">Componentes do Windows de auditoria, armazenar Bloqueador inteligente e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="f5804-124">Audit Windows components, store apps and smart locker.</span></span>|



