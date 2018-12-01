---
title: tipo de enum defenderCloudBlockLevelType
description: Valores possíveis de nível de bloco de nuvem
ms.openlocfilehash: 70e43e9659e7dd7be1d3c0a190e21d80d7b8dc41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038649"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="6545b-103">tipo de enum defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="6545b-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="6545b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6545b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6545b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6545b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6545b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6545b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6545b-107">Valores possíveis de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="6545b-107">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="6545b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6545b-108">Members</span></span>
|<span data-ttu-id="6545b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6545b-109">Member</span></span>|<span data-ttu-id="6545b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6545b-110">Value</span></span>|<span data-ttu-id="6545b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6545b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6545b-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="6545b-112">notConfigured</span></span>|<span data-ttu-id="6545b-113">0</span><span class="sxs-lookup"><span data-stu-id="6545b-113">0</span></span>|<span data-ttu-id="6545b-114">Valor padrão, usa o padrão de bloqueio de antivírus do Windows Defender nível e fornece detecção forte sem aumentar o risco de detecção legítimos arquivos</span><span class="sxs-lookup"><span data-stu-id="6545b-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="6545b-115">high</span><span class="sxs-lookup"><span data-stu-id="6545b-115">high</span></span>|<span data-ttu-id="6545b-116">1</span><span class="sxs-lookup"><span data-stu-id="6545b-116">1</span></span>|<span data-ttu-id="6545b-117">Alta aplica um alto nível de detecção.</span><span class="sxs-lookup"><span data-stu-id="6545b-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="6545b-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="6545b-118">highPlus</span></span>|<span data-ttu-id="6545b-119">2</span><span class="sxs-lookup"><span data-stu-id="6545b-119">2</span></span>|<span data-ttu-id="6545b-120">Alta + usa o alto nível e aplica as medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="6545b-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="6545b-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="6545b-121">zeroTolerance</span></span>|<span data-ttu-id="6545b-122">3</span><span class="sxs-lookup"><span data-stu-id="6545b-122">3</span></span>|<span data-ttu-id="6545b-123">Zero tolerância bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="6545b-123">Zero tolerance blocks all unknown executables</span></span>|





