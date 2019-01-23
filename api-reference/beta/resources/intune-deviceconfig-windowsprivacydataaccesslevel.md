---
title: tipo de enum windowsPrivacyDataAccessLevel
description: Determine o nível de acesso a categoria de dados de privacidade Windows específica.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5d6fed0897b22a6a6b478dc5d2b7954faca42b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410620"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="c8610-103">tipo de enum windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="c8610-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="c8610-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c8610-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c8610-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c8610-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8610-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c8610-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8610-107">Determine o nível de acesso a categoria de dados de privacidade Windows específica.</span><span class="sxs-lookup"><span data-stu-id="c8610-107">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="c8610-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c8610-108">Members</span></span>
|<span data-ttu-id="c8610-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c8610-109">Member</span></span>|<span data-ttu-id="c8610-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c8610-110">Value</span></span>|<span data-ttu-id="c8610-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8610-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8610-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="c8610-112">notConfigured</span></span>|<span data-ttu-id="c8610-113">0</span><span class="sxs-lookup"><span data-stu-id="c8610-113">0</span></span>|<span data-ttu-id="c8610-114">Nenhum nível de acesso não especificado, nenhum propósitos.</span><span class="sxs-lookup"><span data-stu-id="c8610-114">No access level specified, no intents.</span></span> <span data-ttu-id="c8610-115">Dispositivo pode se comportam tanto como UserInControl ou ForceAllow.</span><span class="sxs-lookup"><span data-stu-id="c8610-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="c8610-116">Ele pode depender os dados de privacidade foram acessados, versões do Windows e outros fatores.</span><span class="sxs-lookup"><span data-stu-id="c8610-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="c8610-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="c8610-117">forceAllow</span></span>|<span data-ttu-id="c8610-118">1</span><span class="sxs-lookup"><span data-stu-id="c8610-118">1</span></span>|<span data-ttu-id="c8610-119">Aplicativos poderão acessar os dados de privacidade especificado.</span><span class="sxs-lookup"><span data-stu-id="c8610-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="c8610-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="c8610-120">forceDeny</span></span>|<span data-ttu-id="c8610-121">2</span><span class="sxs-lookup"><span data-stu-id="c8610-121">2</span></span>|<span data-ttu-id="c8610-122">Aplicativos serão negados para acessar os dados de privacidade especificado.</span><span class="sxs-lookup"><span data-stu-id="c8610-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="c8610-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="c8610-123">userInControl</span></span>|<span data-ttu-id="c8610-124">3</span><span class="sxs-lookup"><span data-stu-id="c8610-124">3</span></span>|<span data-ttu-id="c8610-125">Os usuários serão solicitados quando apps tentam acessar os dados de privacidade especificado.</span><span class="sxs-lookup"><span data-stu-id="c8610-125">Users will be prompted when apps try to access specified privacy data.</span></span>|




