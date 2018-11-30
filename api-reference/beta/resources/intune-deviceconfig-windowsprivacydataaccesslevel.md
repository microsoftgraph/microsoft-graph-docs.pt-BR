---
title: tipo de enum windowsPrivacyDataAccessLevel
description: Determine o nível de acesso a categoria de dados de privacidade Windows específica.
ms.openlocfilehash: 09db03706795cc2aba4cc0c93dce87dc7069cd3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040905"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="1b431-103">tipo de enum windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="1b431-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="1b431-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1b431-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b431-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1b431-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b431-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1b431-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b431-107">Determine o nível de acesso a categoria de dados de privacidade Windows específica.</span><span class="sxs-lookup"><span data-stu-id="1b431-107">Determine the access level to specific Windows privacy data category.</span></span>
## <a name="members"></a><span data-ttu-id="1b431-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1b431-108">Members</span></span>
|<span data-ttu-id="1b431-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1b431-109">Member</span></span>|<span data-ttu-id="1b431-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1b431-110">Value</span></span>|<span data-ttu-id="1b431-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b431-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b431-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="1b431-112">notConfigured</span></span>|<span data-ttu-id="1b431-113">0</span><span class="sxs-lookup"><span data-stu-id="1b431-113">0</span></span>|<span data-ttu-id="1b431-114">Nenhum nível de acesso não especificado, nenhum propósitos.</span><span class="sxs-lookup"><span data-stu-id="1b431-114">No access level specified, no intents.</span></span> <span data-ttu-id="1b431-115">Dispositivo pode se comportam tanto como UserInControl ou ForceAllow.</span><span class="sxs-lookup"><span data-stu-id="1b431-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="1b431-116">Ele pode depender os dados de privacidade foram acessados, versões do Windows e outros fatores.</span><span class="sxs-lookup"><span data-stu-id="1b431-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="1b431-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="1b431-117">forceAllow</span></span>|<span data-ttu-id="1b431-118">1</span><span class="sxs-lookup"><span data-stu-id="1b431-118">1</span></span>|<span data-ttu-id="1b431-119">Aplicativos poderão acessar os dados de privacidade especificado.</span><span class="sxs-lookup"><span data-stu-id="1b431-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="1b431-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="1b431-120">forceDeny</span></span>|<span data-ttu-id="1b431-121">2</span><span class="sxs-lookup"><span data-stu-id="1b431-121">2</span></span>|<span data-ttu-id="1b431-122">Aplicativos serão negados para acessar os dados de privacidade especificado.</span><span class="sxs-lookup"><span data-stu-id="1b431-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="1b431-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="1b431-123">userInControl</span></span>|<span data-ttu-id="1b431-124">3</span><span class="sxs-lookup"><span data-stu-id="1b431-124">3</span></span>|<span data-ttu-id="1b431-125">Os usuários serão solicitados quando apps tentam acessar os dados de privacidade especificado.</span><span class="sxs-lookup"><span data-stu-id="1b431-125">Users will be prompted when apps try to access specified privacy data.</span></span>|





