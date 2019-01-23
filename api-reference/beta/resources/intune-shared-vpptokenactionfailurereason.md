---
title: tipo de enum vppTokenActionFailureReason
description: Tipos possíveis razões para uma falha de token de ação do programa de compra de Volume do Apple.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bba4c339b774fd32a852925729e2e158dc13e52d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393141"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="2e99d-103">tipo de enum vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="2e99d-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="2e99d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2e99d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2e99d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2e99d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e99d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2e99d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e99d-107">Tipos possíveis razões para uma falha de token de ação do programa de compra de Volume do Apple.</span><span class="sxs-lookup"><span data-stu-id="2e99d-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="2e99d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2e99d-108">Members</span></span>
|<span data-ttu-id="2e99d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2e99d-109">Member</span></span>|<span data-ttu-id="2e99d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2e99d-110">Value</span></span>|<span data-ttu-id="2e99d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e99d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e99d-112">none</span><span class="sxs-lookup"><span data-stu-id="2e99d-112">none</span></span>|<span data-ttu-id="2e99d-113">0</span><span class="sxs-lookup"><span data-stu-id="2e99d-113">0</span></span>|<span data-ttu-id="2e99d-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2e99d-114">None.</span></span>|
|<span data-ttu-id="2e99d-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="2e99d-115">appleFailure</span></span>|<span data-ttu-id="2e99d-116">1</span><span class="sxs-lookup"><span data-stu-id="2e99d-116">1</span></span>|<span data-ttu-id="2e99d-117">Houve um erro no serviço da Apple.</span><span class="sxs-lookup"><span data-stu-id="2e99d-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="2e99d-118">internalError</span><span class="sxs-lookup"><span data-stu-id="2e99d-118">internalError</span></span>|<span data-ttu-id="2e99d-119">2</span><span class="sxs-lookup"><span data-stu-id="2e99d-119">2</span></span>|<span data-ttu-id="2e99d-120">Houve um erro interno.</span><span class="sxs-lookup"><span data-stu-id="2e99d-120">There was an internal error.</span></span>|
|<span data-ttu-id="2e99d-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="2e99d-121">expiredVppToken</span></span>|<span data-ttu-id="2e99d-122">3</span><span class="sxs-lookup"><span data-stu-id="2e99d-122">3</span></span>|<span data-ttu-id="2e99d-123">Houve um erro, porque o token do programa de compra de Volume do Apple expirou.</span><span class="sxs-lookup"><span data-stu-id="2e99d-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="2e99d-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="2e99d-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="2e99d-125">4</span><span class="sxs-lookup"><span data-stu-id="2e99d-125">4</span></span>|<span data-ttu-id="2e99d-126">Houve um erro, porque o certificado de notificação de Push do Apple Volume compra programa expirado.</span><span class="sxs-lookup"><span data-stu-id="2e99d-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|




