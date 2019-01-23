---
title: tipo de enum deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis de configurações do protetor de credencial.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d8643744e1f5c36cf6c620ac85a6a99c9a77548
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398090"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="1bc3a-103">tipo de enum deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="1bc3a-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="1bc3a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="1bc3a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1bc3a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1bc3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1bc3a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="1bc3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bc3a-107">Valores possíveis de configurações do protetor de credencial.</span><span class="sxs-lookup"><span data-stu-id="1bc3a-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="1bc3a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1bc3a-108">Members</span></span>
|<span data-ttu-id="1bc3a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1bc3a-109">Member</span></span>|<span data-ttu-id="1bc3a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1bc3a-110">Value</span></span>|<span data-ttu-id="1bc3a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bc3a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bc3a-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="1bc3a-112">notConfigured</span></span>|<span data-ttu-id="1bc3a-113">0</span><span class="sxs-lookup"><span data-stu-id="1bc3a-113">0</span></span>|<span data-ttu-id="1bc3a-114">Desativa a credencial Guard remotamente se configurado anteriormente sem bloqueio UEFI.</span><span class="sxs-lookup"><span data-stu-id="1bc3a-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="1bc3a-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="1bc3a-115">enableWithUEFILock</span></span>|<span data-ttu-id="1bc3a-116">1</span><span class="sxs-lookup"><span data-stu-id="1bc3a-116">1</span></span>|<span data-ttu-id="1bc3a-117">Ativa o protetor de credencial com lock UEFI.</span><span class="sxs-lookup"><span data-stu-id="1bc3a-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="1bc3a-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="1bc3a-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="1bc3a-119">2</span><span class="sxs-lookup"><span data-stu-id="1bc3a-119">2</span></span>|<span data-ttu-id="1bc3a-120">Ativa o protetor de credencial sem bloqueio UEFI.</span><span class="sxs-lookup"><span data-stu-id="1bc3a-120">Turns on Credential Guard without UEFI lock.</span></span>|




