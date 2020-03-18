---
title: tipo de enumeração vppTokenActionFailureReason
description: Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8765d0dd62579f470133e81005ff995638e00a5d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767096"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="10566-103">tipo de enumeração vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="10566-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="10566-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10566-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10566-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10566-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10566-106">Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="10566-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="10566-107">Membros</span><span class="sxs-lookup"><span data-stu-id="10566-107">Members</span></span>
|<span data-ttu-id="10566-108">Membro</span><span class="sxs-lookup"><span data-stu-id="10566-108">Member</span></span>|<span data-ttu-id="10566-109">Valor</span><span class="sxs-lookup"><span data-stu-id="10566-109">Value</span></span>|<span data-ttu-id="10566-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="10566-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10566-111">none</span><span class="sxs-lookup"><span data-stu-id="10566-111">none</span></span>|<span data-ttu-id="10566-112">,0</span><span class="sxs-lookup"><span data-stu-id="10566-112">0</span></span>|<span data-ttu-id="10566-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="10566-113">None.</span></span>|
|<span data-ttu-id="10566-114">appleFailure</span><span class="sxs-lookup"><span data-stu-id="10566-114">appleFailure</span></span>|<span data-ttu-id="10566-115">1</span><span class="sxs-lookup"><span data-stu-id="10566-115">1</span></span>|<span data-ttu-id="10566-116">Ocorreu um erro no serviço da Apple.</span><span class="sxs-lookup"><span data-stu-id="10566-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="10566-117">internalError</span><span class="sxs-lookup"><span data-stu-id="10566-117">internalError</span></span>|<span data-ttu-id="10566-118">duas</span><span class="sxs-lookup"><span data-stu-id="10566-118">2</span></span>|<span data-ttu-id="10566-119">Ocorreu um erro interno.</span><span class="sxs-lookup"><span data-stu-id="10566-119">There was an internal error.</span></span>|
|<span data-ttu-id="10566-120">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="10566-120">expiredVppToken</span></span>|<span data-ttu-id="10566-121">3D</span><span class="sxs-lookup"><span data-stu-id="10566-121">3</span></span>|<span data-ttu-id="10566-122">Ocorreu um erro porque o token do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="10566-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="10566-123">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="10566-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="10566-124">4 </span><span class="sxs-lookup"><span data-stu-id="10566-124">4</span></span>|<span data-ttu-id="10566-125">Ocorreu um erro porque o certificado de notificação por push do Apple Volume Purchase Program expirou.</span><span class="sxs-lookup"><span data-stu-id="10566-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|



