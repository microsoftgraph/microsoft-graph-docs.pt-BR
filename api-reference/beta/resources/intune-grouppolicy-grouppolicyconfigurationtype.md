---
title: tipo de enum groupPolicyConfigurationType
description: Tipo de configuração de diretiva de grupo
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 372a5bd5656510c43b388bac128cba4bc46c0988
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429086"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="5a659-103">tipo de enum groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="5a659-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="5a659-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5a659-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5a659-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5a659-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a659-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5a659-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a659-107">Tipo de configuração de diretiva de grupo</span><span class="sxs-lookup"><span data-stu-id="5a659-107">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="5a659-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5a659-108">Members</span></span>
|<span data-ttu-id="5a659-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5a659-109">Member</span></span>|<span data-ttu-id="5a659-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5a659-110">Value</span></span>|<span data-ttu-id="5a659-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a659-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a659-112">Política</span><span class="sxs-lookup"><span data-stu-id="5a659-112">policy</span></span>|<span data-ttu-id="5a659-113">0</span><span class="sxs-lookup"><span data-stu-id="5a659-113">0</span></span>|<span data-ttu-id="5a659-114">O tipo de política não tatuam o valor, o que significa que o valor é removido, permitindo que o valor original de configuração a ser usado.</span><span class="sxs-lookup"><span data-stu-id="5a659-114">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="5a659-115">O tipo de política substitui a definição de configuração de aplicativo para que o aplicativo sempre seja ciente do valor.</span><span class="sxs-lookup"><span data-stu-id="5a659-115">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="5a659-116">O tipo de política impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a659-116">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="5a659-117">preference</span><span class="sxs-lookup"><span data-stu-id="5a659-117">preference</span></span>|<span data-ttu-id="5a659-118">1</span><span class="sxs-lookup"><span data-stu-id="5a659-118">1</span></span>|<span data-ttu-id="5a659-119">O tipo de preferência tatuam o valor, o que significa que o valor não é removido do registro.</span><span class="sxs-lookup"><span data-stu-id="5a659-119">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="5a659-120">O tipo de preferência substituirá o usuário configurado valor e não retém o valor anterior.</span><span class="sxs-lookup"><span data-stu-id="5a659-120">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="5a659-121">O tipo de preferência não impede que o usuário modificar o valor por meio da interface do usuário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a659-121">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|




