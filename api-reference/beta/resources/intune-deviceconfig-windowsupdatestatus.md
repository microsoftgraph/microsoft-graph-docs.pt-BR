---
title: tipo de enum windowsUpdateStatus
description: Windows update para os estados de dispositivo de configuração de negócios
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74493359eeccdbc6df1c351ecec771b5990649b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431294"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="eacf8-103">tipo de enum windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="eacf8-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="eacf8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="eacf8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eacf8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eacf8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eacf8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="eacf8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eacf8-107">Windows update para os estados de dispositivo de configuração de negócios</span><span class="sxs-lookup"><span data-stu-id="eacf8-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="eacf8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="eacf8-108">Members</span></span>
|<span data-ttu-id="eacf8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="eacf8-109">Member</span></span>|<span data-ttu-id="eacf8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="eacf8-110">Value</span></span>|<span data-ttu-id="eacf8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eacf8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eacf8-112">upToDate</span><span class="sxs-lookup"><span data-stu-id="eacf8-112">upToDate</span></span>|<span data-ttu-id="eacf8-113">0</span><span class="sxs-lookup"><span data-stu-id="eacf8-113">0</span></span>|<span data-ttu-id="eacf8-114">Não existem atualizações pendentes, não pendentes atualizações de reinicialização e falhas de atualização.</span><span class="sxs-lookup"><span data-stu-id="eacf8-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="eacf8-115">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="eacf8-115">pendingInstallation</span></span>|<span data-ttu-id="eacf8-116">1</span><span class="sxs-lookup"><span data-stu-id="eacf8-116">1</span></span>|<span data-ttu-id="eacf8-117">Há atualizações da instalação que inclui atualizações que não estão aprovadas pendente.</span><span class="sxs-lookup"><span data-stu-id="eacf8-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="eacf8-118">Há atualizações sem reinicialização pendente, não há falhas de atualização.</span><span class="sxs-lookup"><span data-stu-id="eacf8-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="eacf8-119">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="eacf8-119">pendingReboot</span></span>|<span data-ttu-id="eacf8-120">2</span><span class="sxs-lookup"><span data-stu-id="eacf8-120">2</span></span>|<span data-ttu-id="eacf8-121">Há atualizações que exige reinicialização.</span><span class="sxs-lookup"><span data-stu-id="eacf8-121">There are updates that requires reboot.</span></span> <span data-ttu-id="eacf8-122">Não há falhas de atualização.</span><span class="sxs-lookup"><span data-stu-id="eacf8-122">There are not failed updates.</span></span>|
|<span data-ttu-id="eacf8-123">Falha</span><span class="sxs-lookup"><span data-stu-id="eacf8-123">failed</span></span>|<span data-ttu-id="eacf8-124">3</span><span class="sxs-lookup"><span data-stu-id="eacf8-124">3</span></span>|<span data-ttu-id="eacf8-125">Há atualizações Falha ao instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eacf8-125">There are updates failed to install on the device.</span></span>|




