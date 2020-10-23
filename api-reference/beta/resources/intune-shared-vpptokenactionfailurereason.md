---
title: tipo de enumeração vppTokenActionFailureReason
description: Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 250b1d3939cb06947b60ea45de71d0843830effc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727103"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="aa801-103">tipo de enumeração vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="aa801-103">vppTokenActionFailureReason enum type</span></span>

<span data-ttu-id="aa801-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa801-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa801-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aa801-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa801-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa801-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa801-107">Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="aa801-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="aa801-108">Membros</span><span class="sxs-lookup"><span data-stu-id="aa801-108">Members</span></span>
|<span data-ttu-id="aa801-109">Membro</span><span class="sxs-lookup"><span data-stu-id="aa801-109">Member</span></span>|<span data-ttu-id="aa801-110">Valor</span><span class="sxs-lookup"><span data-stu-id="aa801-110">Value</span></span>|<span data-ttu-id="aa801-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa801-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa801-112">none</span><span class="sxs-lookup"><span data-stu-id="aa801-112">none</span></span>|<span data-ttu-id="aa801-113">,0</span><span class="sxs-lookup"><span data-stu-id="aa801-113">0</span></span>|<span data-ttu-id="aa801-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aa801-114">None.</span></span>|
|<span data-ttu-id="aa801-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="aa801-115">appleFailure</span></span>|<span data-ttu-id="aa801-116">1</span><span class="sxs-lookup"><span data-stu-id="aa801-116">1</span></span>|<span data-ttu-id="aa801-117">Ocorreu um erro no serviço da Apple.</span><span class="sxs-lookup"><span data-stu-id="aa801-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="aa801-118">internalError</span><span class="sxs-lookup"><span data-stu-id="aa801-118">internalError</span></span>|<span data-ttu-id="aa801-119">duas</span><span class="sxs-lookup"><span data-stu-id="aa801-119">2</span></span>|<span data-ttu-id="aa801-120">Ocorreu um erro interno.</span><span class="sxs-lookup"><span data-stu-id="aa801-120">There was an internal error.</span></span>|
|<span data-ttu-id="aa801-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="aa801-121">expiredVppToken</span></span>|<span data-ttu-id="aa801-122">3D</span><span class="sxs-lookup"><span data-stu-id="aa801-122">3</span></span>|<span data-ttu-id="aa801-123">Ocorreu um erro porque o token do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="aa801-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="aa801-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="aa801-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="aa801-125">4 </span><span class="sxs-lookup"><span data-stu-id="aa801-125">4</span></span>|<span data-ttu-id="aa801-126">Ocorreu um erro porque o certificado de notificação por push do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="aa801-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





