---
title: tipo de enum windowsPrivacyDataAccessLevel
description: Determine o nível de acesso a categoria de dados de privacidade Windows específica.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 64db5eb78708a0cfa835bd695ba01b2c267fc4fd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959311"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="037be-103">tipo de enum windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="037be-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="037be-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="037be-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="037be-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="037be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="037be-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="037be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="037be-107">Determine o nível de acesso a categoria de dados de privacidade Windows específica.</span><span class="sxs-lookup"><span data-stu-id="037be-107">Determine the access level to specific Windows privacy data category.</span></span>
## <a name="members"></a><span data-ttu-id="037be-108">Membros</span><span class="sxs-lookup"><span data-stu-id="037be-108">Members</span></span>
|<span data-ttu-id="037be-109">Membro</span><span class="sxs-lookup"><span data-stu-id="037be-109">Member</span></span>|<span data-ttu-id="037be-110">Valor</span><span class="sxs-lookup"><span data-stu-id="037be-110">Value</span></span>|<span data-ttu-id="037be-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="037be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="037be-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="037be-112">notConfigured</span></span>|<span data-ttu-id="037be-113">0</span><span class="sxs-lookup"><span data-stu-id="037be-113">0</span></span>|<span data-ttu-id="037be-114">Nenhum nível de acesso não especificado, nenhum propósitos.</span><span class="sxs-lookup"><span data-stu-id="037be-114">No access level specified, no intents.</span></span> <span data-ttu-id="037be-115">Dispositivo pode se comportam tanto como UserInControl ou ForceAllow.</span><span class="sxs-lookup"><span data-stu-id="037be-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="037be-116">Ele pode depender os dados de privacidade foram acessados, versões do Windows e outros fatores.</span><span class="sxs-lookup"><span data-stu-id="037be-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="037be-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="037be-117">forceAllow</span></span>|<span data-ttu-id="037be-118">1</span><span class="sxs-lookup"><span data-stu-id="037be-118">1</span></span>|<span data-ttu-id="037be-119">Aplicativos poderão acessar os dados de privacidade especificado.</span><span class="sxs-lookup"><span data-stu-id="037be-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="037be-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="037be-120">forceDeny</span></span>|<span data-ttu-id="037be-121">2</span><span class="sxs-lookup"><span data-stu-id="037be-121">2</span></span>|<span data-ttu-id="037be-122">Aplicativos serão negados para acessar os dados de privacidade especificado.</span><span class="sxs-lookup"><span data-stu-id="037be-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="037be-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="037be-123">userInControl</span></span>|<span data-ttu-id="037be-124">3</span><span class="sxs-lookup"><span data-stu-id="037be-124">3</span></span>|<span data-ttu-id="037be-125">Os usuários serão solicitados quando apps tentam acessar os dados de privacidade especificado.</span><span class="sxs-lookup"><span data-stu-id="037be-125">Users will be prompted when apps try to access specified privacy data.</span></span>|





