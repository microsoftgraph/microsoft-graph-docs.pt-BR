---
title: tipo de enum deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis de configurações do protetor de credencial.
author: tfitzmac
ms.openlocfilehash: 6f6c952d1c480d42db45de6345eba883ff5848a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346960"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="fce5b-103">tipo de enum deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="fce5b-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="fce5b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fce5b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fce5b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fce5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fce5b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fce5b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fce5b-107">Valores possíveis de configurações do protetor de credencial.</span><span class="sxs-lookup"><span data-stu-id="fce5b-107">Possible values of Credential Guard settings.</span></span>
## <a name="members"></a><span data-ttu-id="fce5b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="fce5b-108">Members</span></span>
|<span data-ttu-id="fce5b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="fce5b-109">Member</span></span>|<span data-ttu-id="fce5b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="fce5b-110">Value</span></span>|<span data-ttu-id="fce5b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fce5b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fce5b-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="fce5b-112">notConfigured</span></span>|<span data-ttu-id="fce5b-113">0</span><span class="sxs-lookup"><span data-stu-id="fce5b-113">0</span></span>|<span data-ttu-id="fce5b-114">Desativa a credencial Guard remotamente se configurado anteriormente sem bloqueio UEFI.</span><span class="sxs-lookup"><span data-stu-id="fce5b-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="fce5b-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="fce5b-115">enableWithUEFILock</span></span>|<span data-ttu-id="fce5b-116">1</span><span class="sxs-lookup"><span data-stu-id="fce5b-116">1</span></span>|<span data-ttu-id="fce5b-117">Ativa o protetor de credencial com lock UEFI.</span><span class="sxs-lookup"><span data-stu-id="fce5b-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="fce5b-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="fce5b-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="fce5b-119">2</span><span class="sxs-lookup"><span data-stu-id="fce5b-119">2</span></span>|<span data-ttu-id="fce5b-120">Ativa o protetor de credencial sem bloqueio UEFI.</span><span class="sxs-lookup"><span data-stu-id="fce5b-120">Turns on Credential Guard without UEFI lock.</span></span>|





