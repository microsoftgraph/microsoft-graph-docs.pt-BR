---
title: tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis das configurações do Credential Guard.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 97f04bbf16d93602be466e4dc5fe4986cc26319e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530141"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="f4a82-103">tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="f4a82-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="f4a82-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f4a82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4a82-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4a82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4a82-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4a82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4a82-107">Valores possíveis das configurações do Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="f4a82-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="f4a82-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f4a82-108">Members</span></span>
|<span data-ttu-id="f4a82-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f4a82-109">Member</span></span>|<span data-ttu-id="f4a82-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f4a82-110">Value</span></span>|<span data-ttu-id="f4a82-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4a82-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4a82-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f4a82-112">notConfigured</span></span>|<span data-ttu-id="f4a82-113">,0</span><span class="sxs-lookup"><span data-stu-id="f4a82-113">0</span></span>|<span data-ttu-id="f4a82-114">Desativa o Credential Guard remotamente, se configurado anteriormente sem bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="f4a82-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="f4a82-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="f4a82-115">enableWithUEFILock</span></span>|<span data-ttu-id="f4a82-116">1 </span><span class="sxs-lookup"><span data-stu-id="f4a82-116">1</span></span>|<span data-ttu-id="f4a82-117">Ativa o Credential Guard com bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="f4a82-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="f4a82-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="f4a82-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="f4a82-119">2 </span><span class="sxs-lookup"><span data-stu-id="f4a82-119">2</span></span>|<span data-ttu-id="f4a82-120">Ativa o Credential Guard sem bloqueio de UEFI.</span><span class="sxs-lookup"><span data-stu-id="f4a82-120">Turns on Credential Guard without UEFI lock.</span></span>|



