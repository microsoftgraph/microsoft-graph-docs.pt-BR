---
title: tipo de enumeração vppTokenActionFailureReason
description: Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8b7df30d2673696200b29e14d7c450c41d5a5f8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523503"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="93f8c-103">tipo de enumeração vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="93f8c-103">vppTokenActionFailureReason enum type</span></span>

<span data-ttu-id="93f8c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="93f8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93f8c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93f8c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93f8c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93f8c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93f8c-107">Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="93f8c-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="93f8c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="93f8c-108">Members</span></span>
|<span data-ttu-id="93f8c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="93f8c-109">Member</span></span>|<span data-ttu-id="93f8c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="93f8c-110">Value</span></span>|<span data-ttu-id="93f8c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="93f8c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93f8c-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="93f8c-112">none</span></span>|<span data-ttu-id="93f8c-113">,0</span><span class="sxs-lookup"><span data-stu-id="93f8c-113">0</span></span>|<span data-ttu-id="93f8c-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="93f8c-114">None.</span></span>|
|<span data-ttu-id="93f8c-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="93f8c-115">appleFailure</span></span>|<span data-ttu-id="93f8c-116">1 </span><span class="sxs-lookup"><span data-stu-id="93f8c-116">1</span></span>|<span data-ttu-id="93f8c-117">Ocorreu um erro no serviço da Apple.</span><span class="sxs-lookup"><span data-stu-id="93f8c-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="93f8c-118">internalError</span><span class="sxs-lookup"><span data-stu-id="93f8c-118">internalError</span></span>|<span data-ttu-id="93f8c-119">2 </span><span class="sxs-lookup"><span data-stu-id="93f8c-119">2</span></span>|<span data-ttu-id="93f8c-120">Ocorreu um erro interno.</span><span class="sxs-lookup"><span data-stu-id="93f8c-120">There was an internal error.</span></span>|
|<span data-ttu-id="93f8c-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="93f8c-121">expiredVppToken</span></span>|<span data-ttu-id="93f8c-122">3 </span><span class="sxs-lookup"><span data-stu-id="93f8c-122">3</span></span>|<span data-ttu-id="93f8c-123">Ocorreu um erro porque o token do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="93f8c-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="93f8c-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="93f8c-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="93f8c-125">4 </span><span class="sxs-lookup"><span data-stu-id="93f8c-125">4</span></span>|<span data-ttu-id="93f8c-126">Ocorreu um erro porque o certificado de notificação por push do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="93f8c-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|



