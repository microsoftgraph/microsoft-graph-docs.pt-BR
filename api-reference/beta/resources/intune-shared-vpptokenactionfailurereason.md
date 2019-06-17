---
title: tipo de enumeração vppTokenActionFailureReason
description: Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0f8aacb6fc6f95b8c8085a78ed2851b16622357
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990985"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="e14e7-103">tipo de enumeração vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="e14e7-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="e14e7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e14e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e14e7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e14e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e14e7-106">Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="e14e7-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="e14e7-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e14e7-107">Members</span></span>
|<span data-ttu-id="e14e7-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e14e7-108">Member</span></span>|<span data-ttu-id="e14e7-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e14e7-109">Value</span></span>|<span data-ttu-id="e14e7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e14e7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e14e7-111">none</span><span class="sxs-lookup"><span data-stu-id="e14e7-111">none</span></span>|<span data-ttu-id="e14e7-112">,0</span><span class="sxs-lookup"><span data-stu-id="e14e7-112">0</span></span>|<span data-ttu-id="e14e7-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e14e7-113">None.</span></span>|
|<span data-ttu-id="e14e7-114">appleFailure</span><span class="sxs-lookup"><span data-stu-id="e14e7-114">appleFailure</span></span>|<span data-ttu-id="e14e7-115">1</span><span class="sxs-lookup"><span data-stu-id="e14e7-115">1</span></span>|<span data-ttu-id="e14e7-116">Ocorreu um erro no serviço da Apple.</span><span class="sxs-lookup"><span data-stu-id="e14e7-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="e14e7-117">internalError</span><span class="sxs-lookup"><span data-stu-id="e14e7-117">internalError</span></span>|<span data-ttu-id="e14e7-118">duas</span><span class="sxs-lookup"><span data-stu-id="e14e7-118">2</span></span>|<span data-ttu-id="e14e7-119">Ocorreu um erro interno.</span><span class="sxs-lookup"><span data-stu-id="e14e7-119">There was an internal error.</span></span>|
|<span data-ttu-id="e14e7-120">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="e14e7-120">expiredVppToken</span></span>|<span data-ttu-id="e14e7-121">3D</span><span class="sxs-lookup"><span data-stu-id="e14e7-121">3</span></span>|<span data-ttu-id="e14e7-122">Ocorreu um erro porque o token do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="e14e7-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="e14e7-123">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="e14e7-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="e14e7-124">quatro</span><span class="sxs-lookup"><span data-stu-id="e14e7-124">4</span></span>|<span data-ttu-id="e14e7-125">Ocorreu um erro porque o certificado de notificação por push do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="e14e7-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





