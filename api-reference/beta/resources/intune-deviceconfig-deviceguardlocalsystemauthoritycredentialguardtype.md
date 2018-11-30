---
title: tipo de enum deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis de configurações do protetor de credencial.
ms.openlocfilehash: 73668ec4d6d5026402757fae3443da4540fb374c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033188"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="1e4e5-103">tipo de enum deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="1e4e5-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="1e4e5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1e4e5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e4e5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1e4e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e4e5-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1e4e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e4e5-107">Valores possíveis de configurações do protetor de credencial.</span><span class="sxs-lookup"><span data-stu-id="1e4e5-107">Possible values of Credential Guard settings.</span></span>
## <a name="members"></a><span data-ttu-id="1e4e5-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1e4e5-108">Members</span></span>
|<span data-ttu-id="1e4e5-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1e4e5-109">Member</span></span>|<span data-ttu-id="1e4e5-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1e4e5-110">Value</span></span>|<span data-ttu-id="1e4e5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e4e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e4e5-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="1e4e5-112">notConfigured</span></span>|<span data-ttu-id="1e4e5-113">0</span><span class="sxs-lookup"><span data-stu-id="1e4e5-113">0</span></span>|<span data-ttu-id="1e4e5-114">Desativa a credencial Guard remotamente se configurado anteriormente sem bloqueio UEFI.</span><span class="sxs-lookup"><span data-stu-id="1e4e5-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="1e4e5-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="1e4e5-115">enableWithUEFILock</span></span>|<span data-ttu-id="1e4e5-116">1</span><span class="sxs-lookup"><span data-stu-id="1e4e5-116">1</span></span>|<span data-ttu-id="1e4e5-117">Ativa o protetor de credencial com lock UEFI.</span><span class="sxs-lookup"><span data-stu-id="1e4e5-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="1e4e5-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="1e4e5-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="1e4e5-119">2</span><span class="sxs-lookup"><span data-stu-id="1e4e5-119">2</span></span>|<span data-ttu-id="1e4e5-120">Ativa o protetor de credencial sem bloqueio UEFI.</span><span class="sxs-lookup"><span data-stu-id="1e4e5-120">Turns on Credential Guard without UEFI lock.</span></span>|





