---
title: tipo de enumeração vppTokenActionFailureReason
description: Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9adb896d384be99496c016ef3bd39b02ff1a28e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548254"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="e1af4-103">tipo de enumeração vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="e1af4-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="e1af4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1af4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1af4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1af4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1af4-106">Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="e1af4-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="e1af4-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e1af4-107">Members</span></span>
|<span data-ttu-id="e1af4-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e1af4-108">Member</span></span>|<span data-ttu-id="e1af4-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e1af4-109">Value</span></span>|<span data-ttu-id="e1af4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1af4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1af4-111">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e1af4-111">none</span></span>|<span data-ttu-id="e1af4-112">,0</span><span class="sxs-lookup"><span data-stu-id="e1af4-112">0</span></span>|<span data-ttu-id="e1af4-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e1af4-113">None.</span></span>|
|<span data-ttu-id="e1af4-114">appleFailure</span><span class="sxs-lookup"><span data-stu-id="e1af4-114">appleFailure</span></span>|<span data-ttu-id="e1af4-115">1 </span><span class="sxs-lookup"><span data-stu-id="e1af4-115">1</span></span>|<span data-ttu-id="e1af4-116">Ocorreu um erro no serviço da Apple.</span><span class="sxs-lookup"><span data-stu-id="e1af4-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="e1af4-117">internalError</span><span class="sxs-lookup"><span data-stu-id="e1af4-117">internalError</span></span>|<span data-ttu-id="e1af4-118">2 </span><span class="sxs-lookup"><span data-stu-id="e1af4-118">2</span></span>|<span data-ttu-id="e1af4-119">Ocorreu um erro interno.</span><span class="sxs-lookup"><span data-stu-id="e1af4-119">There was an internal error.</span></span>|
|<span data-ttu-id="e1af4-120">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="e1af4-120">expiredVppToken</span></span>|<span data-ttu-id="e1af4-121">3 </span><span class="sxs-lookup"><span data-stu-id="e1af4-121">3</span></span>|<span data-ttu-id="e1af4-122">Ocorreu um erro porque o token do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="e1af4-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="e1af4-123">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="e1af4-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="e1af4-124">4 </span><span class="sxs-lookup"><span data-stu-id="e1af4-124">4</span></span>|<span data-ttu-id="e1af4-125">Ocorreu um erro porque o certificado de notificação por push do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="e1af4-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





