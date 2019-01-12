---
title: tipo de enum vppTokenActionFailureReason
description: Tipos possíveis razões para uma falha de token de ação do programa de compra de Volume do Apple.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: baf33c29a822cc725c66ff6a3a7d796e57e63693
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961159"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="37ba4-103">tipo de enum vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="37ba4-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="37ba4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="37ba4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37ba4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="37ba4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37ba4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="37ba4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37ba4-107">Tipos possíveis razões para uma falha de token de ação do programa de compra de Volume do Apple.</span><span class="sxs-lookup"><span data-stu-id="37ba4-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>
## <a name="members"></a><span data-ttu-id="37ba4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="37ba4-108">Members</span></span>
|<span data-ttu-id="37ba4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="37ba4-109">Member</span></span>|<span data-ttu-id="37ba4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="37ba4-110">Value</span></span>|<span data-ttu-id="37ba4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="37ba4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37ba4-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="37ba4-112">none</span></span>|<span data-ttu-id="37ba4-113">0</span><span class="sxs-lookup"><span data-stu-id="37ba4-113">0</span></span>|<span data-ttu-id="37ba4-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="37ba4-114">None.</span></span>|
|<span data-ttu-id="37ba4-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="37ba4-115">appleFailure</span></span>|<span data-ttu-id="37ba4-116">1</span><span class="sxs-lookup"><span data-stu-id="37ba4-116">1</span></span>|<span data-ttu-id="37ba4-117">Houve um erro no serviço da Apple.</span><span class="sxs-lookup"><span data-stu-id="37ba4-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="37ba4-118">internalError</span><span class="sxs-lookup"><span data-stu-id="37ba4-118">internalError</span></span>|<span data-ttu-id="37ba4-119">2</span><span class="sxs-lookup"><span data-stu-id="37ba4-119">2</span></span>|<span data-ttu-id="37ba4-120">Houve um erro interno.</span><span class="sxs-lookup"><span data-stu-id="37ba4-120">There was an internal error.</span></span>|
|<span data-ttu-id="37ba4-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="37ba4-121">expiredVppToken</span></span>|<span data-ttu-id="37ba4-122">3</span><span class="sxs-lookup"><span data-stu-id="37ba4-122">3</span></span>|<span data-ttu-id="37ba4-123">Houve um erro, porque o token do programa de compra de Volume do Apple expirou.</span><span class="sxs-lookup"><span data-stu-id="37ba4-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="37ba4-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="37ba4-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="37ba4-125">4</span><span class="sxs-lookup"><span data-stu-id="37ba4-125">4</span></span>|<span data-ttu-id="37ba4-126">Houve um erro, porque o certificado de notificação de Push do Apple Volume compra programa expirado.</span><span class="sxs-lookup"><span data-stu-id="37ba4-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





