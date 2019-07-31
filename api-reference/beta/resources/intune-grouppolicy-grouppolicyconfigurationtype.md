---
title: tipo de enumeração groupPolicyConfigurationType
description: Tipo de configuração da política de grupo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6e0e7f2b1a9c7817af614c2753e4e5fcfe0fe2c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011005"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="30038-103">tipo de enumeração groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="30038-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="30038-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30038-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30038-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30038-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30038-106">Tipo de configuração da política de grupo</span><span class="sxs-lookup"><span data-stu-id="30038-106">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="30038-107">Membros</span><span class="sxs-lookup"><span data-stu-id="30038-107">Members</span></span>
|<span data-ttu-id="30038-108">Membro</span><span class="sxs-lookup"><span data-stu-id="30038-108">Member</span></span>|<span data-ttu-id="30038-109">Valor</span><span class="sxs-lookup"><span data-stu-id="30038-109">Value</span></span>|<span data-ttu-id="30038-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="30038-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30038-111">política</span><span class="sxs-lookup"><span data-stu-id="30038-111">policy</span></span>|<span data-ttu-id="30038-112">,0</span><span class="sxs-lookup"><span data-stu-id="30038-112">0</span></span>|<span data-ttu-id="30038-113">O tipo de política não é de Tattoo o valor, o que significa que o valor é removido, permitindo que o valor de configuração original seja usado.</span><span class="sxs-lookup"><span data-stu-id="30038-113">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="30038-114">O tipo de política substitui a definição de configuração de aplicativo para que o aplicativo sempre saiba o valor.</span><span class="sxs-lookup"><span data-stu-id="30038-114">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="30038-115">O tipo de política impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30038-115">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="30038-116">preferência</span><span class="sxs-lookup"><span data-stu-id="30038-116">preference</span></span>|<span data-ttu-id="30038-117">1</span><span class="sxs-lookup"><span data-stu-id="30038-117">1</span></span>|<span data-ttu-id="30038-118">O tipo de preferência tem o valor de Tattoo, o que significa que o valor não é removido do registro.</span><span class="sxs-lookup"><span data-stu-id="30038-118">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="30038-119">O tipo de preferência substituirá o valor configurado pelo usuário e não manterá o valor anterior.</span><span class="sxs-lookup"><span data-stu-id="30038-119">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="30038-120">O tipo de preferência não impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30038-120">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|





