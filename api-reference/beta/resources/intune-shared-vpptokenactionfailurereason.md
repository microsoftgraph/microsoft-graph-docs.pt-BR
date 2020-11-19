---
title: tipo de enumeração vppTokenActionFailureReason
description: Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ad2151be841133b7fbbbd6bc858e9ecdf3e611d6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271678"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="b8e2b-103">tipo de enumeração vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="b8e2b-103">vppTokenActionFailureReason enum type</span></span>

<span data-ttu-id="b8e2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8e2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8e2b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8e2b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8e2b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8e2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8e2b-107">Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b8e2b-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="b8e2b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b8e2b-108">Members</span></span>
|<span data-ttu-id="b8e2b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b8e2b-109">Member</span></span>|<span data-ttu-id="b8e2b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b8e2b-110">Value</span></span>|<span data-ttu-id="b8e2b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8e2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8e2b-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="b8e2b-112">none</span></span>|<span data-ttu-id="b8e2b-113">,0</span><span class="sxs-lookup"><span data-stu-id="b8e2b-113">0</span></span>|<span data-ttu-id="b8e2b-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b8e2b-114">None.</span></span>|
|<span data-ttu-id="b8e2b-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="b8e2b-115">appleFailure</span></span>|<span data-ttu-id="b8e2b-116">1</span><span class="sxs-lookup"><span data-stu-id="b8e2b-116">1</span></span>|<span data-ttu-id="b8e2b-117">Ocorreu um erro no serviço da Apple.</span><span class="sxs-lookup"><span data-stu-id="b8e2b-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="b8e2b-118">internalError</span><span class="sxs-lookup"><span data-stu-id="b8e2b-118">internalError</span></span>|<span data-ttu-id="b8e2b-119">duas</span><span class="sxs-lookup"><span data-stu-id="b8e2b-119">2</span></span>|<span data-ttu-id="b8e2b-120">Ocorreu um erro interno.</span><span class="sxs-lookup"><span data-stu-id="b8e2b-120">There was an internal error.</span></span>|
|<span data-ttu-id="b8e2b-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="b8e2b-121">expiredVppToken</span></span>|<span data-ttu-id="b8e2b-122">3D</span><span class="sxs-lookup"><span data-stu-id="b8e2b-122">3</span></span>|<span data-ttu-id="b8e2b-123">Ocorreu um erro porque o token do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="b8e2b-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="b8e2b-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="b8e2b-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="b8e2b-125">4 </span><span class="sxs-lookup"><span data-stu-id="b8e2b-125">4</span></span>|<span data-ttu-id="b8e2b-126">Ocorreu um erro porque o certificado de notificação por push do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="b8e2b-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|




