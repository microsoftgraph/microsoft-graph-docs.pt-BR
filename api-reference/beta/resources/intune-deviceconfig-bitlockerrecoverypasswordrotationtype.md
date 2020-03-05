---
title: tipo de enumeração bitLockerRecoveryPasswordRotationType
description: Tipo de rotação da senha de recuperação do BitLocker
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 989690620e6be54caa35e02be0920f15a7d2787b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527031"
---
# <a name="bitlockerrecoverypasswordrotationtype-enum-type"></a><span data-ttu-id="c4822-103">tipo de enumeração bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="c4822-103">bitLockerRecoveryPasswordRotationType enum type</span></span>

<span data-ttu-id="c4822-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c4822-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4822-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4822-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4822-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4822-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4822-107">Tipo de rotação da senha de recuperação do BitLocker</span><span class="sxs-lookup"><span data-stu-id="c4822-107">BitLocker recovery password rotation type</span></span>

## <a name="members"></a><span data-ttu-id="c4822-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c4822-108">Members</span></span>
|<span data-ttu-id="c4822-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c4822-109">Member</span></span>|<span data-ttu-id="c4822-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c4822-110">Value</span></span>|<span data-ttu-id="c4822-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4822-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4822-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c4822-112">notConfigured</span></span>|<span data-ttu-id="c4822-113">,0</span><span class="sxs-lookup"><span data-stu-id="c4822-113">0</span></span>|<span data-ttu-id="c4822-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="c4822-114">Not configured</span></span>|
|<span data-ttu-id="c4822-115">deficiência</span><span class="sxs-lookup"><span data-stu-id="c4822-115">disabled</span></span>|<span data-ttu-id="c4822-116">1 </span><span class="sxs-lookup"><span data-stu-id="c4822-116">1</span></span>|<span data-ttu-id="c4822-117">Rotação da senha de recuperação desativada</span><span class="sxs-lookup"><span data-stu-id="c4822-117">Recovery password rotation off</span></span>|
|<span data-ttu-id="c4822-118">enabledForAzureAd</span><span class="sxs-lookup"><span data-stu-id="c4822-118">enabledForAzureAd</span></span>|<span data-ttu-id="c4822-119">2 </span><span class="sxs-lookup"><span data-stu-id="c4822-119">2</span></span>|<span data-ttu-id="c4822-120">Rotação da senha de recuperação em dispositivos ingressados no Azure AD</span><span class="sxs-lookup"><span data-stu-id="c4822-120">Recovery password rotation on for Azure AD joined devices</span></span>|
|<span data-ttu-id="c4822-121">enabledForAzureAdAndHybrid</span><span class="sxs-lookup"><span data-stu-id="c4822-121">enabledForAzureAdAndHybrid</span></span>|<span data-ttu-id="c4822-122">3 </span><span class="sxs-lookup"><span data-stu-id="c4822-122">3</span></span>|<span data-ttu-id="c4822-123">Rotação da senha de recuperação para os dispositivos ingressados e híbridos do Azure AD</span><span class="sxs-lookup"><span data-stu-id="c4822-123">Recovery password rotation on for both Azure AD joined and hybrid joined devices</span></span>|



