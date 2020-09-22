---
title: tipo de enumeração vppTokenActionFailureReason
description: Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 883772d99077e8587ba5467ec8c9492eddfb62e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070671"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="d312f-103">tipo de enumeração vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="d312f-103">vppTokenActionFailureReason enum type</span></span>

<span data-ttu-id="d312f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d312f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d312f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d312f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d312f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d312f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d312f-107">Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d312f-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="d312f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d312f-108">Members</span></span>
|<span data-ttu-id="d312f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d312f-109">Member</span></span>|<span data-ttu-id="d312f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d312f-110">Value</span></span>|<span data-ttu-id="d312f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d312f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d312f-112">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d312f-112">none</span></span>|<span data-ttu-id="d312f-113">,0</span><span class="sxs-lookup"><span data-stu-id="d312f-113">0</span></span>|<span data-ttu-id="d312f-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d312f-114">None.</span></span>|
|<span data-ttu-id="d312f-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="d312f-115">appleFailure</span></span>|<span data-ttu-id="d312f-116">1 </span><span class="sxs-lookup"><span data-stu-id="d312f-116">1</span></span>|<span data-ttu-id="d312f-117">Ocorreu um erro no serviço da Apple.</span><span class="sxs-lookup"><span data-stu-id="d312f-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="d312f-118">internalError</span><span class="sxs-lookup"><span data-stu-id="d312f-118">internalError</span></span>|<span data-ttu-id="d312f-119">2 </span><span class="sxs-lookup"><span data-stu-id="d312f-119">2</span></span>|<span data-ttu-id="d312f-120">Ocorreu um erro interno.</span><span class="sxs-lookup"><span data-stu-id="d312f-120">There was an internal error.</span></span>|
|<span data-ttu-id="d312f-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="d312f-121">expiredVppToken</span></span>|<span data-ttu-id="d312f-122">3 </span><span class="sxs-lookup"><span data-stu-id="d312f-122">3</span></span>|<span data-ttu-id="d312f-123">Ocorreu um erro porque o token do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="d312f-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="d312f-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d312f-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="d312f-125">4 </span><span class="sxs-lookup"><span data-stu-id="d312f-125">4</span></span>|<span data-ttu-id="d312f-126">Ocorreu um erro porque o certificado de notificação por push do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="d312f-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|






