---
title: tipo de enum defenderCloudBlockLevelType
description: Valores possíveis de nível de bloco de nuvem
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 51ed838b6abaaf36a69230b566c01b8d496c2a70
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872069"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="92bb6-103">tipo de enum defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="92bb6-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="92bb6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="92bb6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92bb6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="92bb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92bb6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="92bb6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92bb6-107">Valores possíveis de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="92bb6-107">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="92bb6-108">Membros</span><span class="sxs-lookup"><span data-stu-id="92bb6-108">Members</span></span>
|<span data-ttu-id="92bb6-109">Membro</span><span class="sxs-lookup"><span data-stu-id="92bb6-109">Member</span></span>|<span data-ttu-id="92bb6-110">Valor</span><span class="sxs-lookup"><span data-stu-id="92bb6-110">Value</span></span>|<span data-ttu-id="92bb6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="92bb6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92bb6-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="92bb6-112">notConfigured</span></span>|<span data-ttu-id="92bb6-113">0</span><span class="sxs-lookup"><span data-stu-id="92bb6-113">0</span></span>|<span data-ttu-id="92bb6-114">Valor padrão, usa o padrão de bloqueio de antivírus do Windows Defender nível e fornece detecção forte sem aumentar o risco de detecção legítimos arquivos</span><span class="sxs-lookup"><span data-stu-id="92bb6-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="92bb6-115">high</span><span class="sxs-lookup"><span data-stu-id="92bb6-115">high</span></span>|<span data-ttu-id="92bb6-116">1</span><span class="sxs-lookup"><span data-stu-id="92bb6-116">1</span></span>|<span data-ttu-id="92bb6-117">Alta aplica um alto nível de detecção.</span><span class="sxs-lookup"><span data-stu-id="92bb6-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="92bb6-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="92bb6-118">highPlus</span></span>|<span data-ttu-id="92bb6-119">2</span><span class="sxs-lookup"><span data-stu-id="92bb6-119">2</span></span>|<span data-ttu-id="92bb6-120">Alta + usa o alto nível e aplica as medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="92bb6-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="92bb6-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="92bb6-121">zeroTolerance</span></span>|<span data-ttu-id="92bb6-122">3</span><span class="sxs-lookup"><span data-stu-id="92bb6-122">3</span></span>|<span data-ttu-id="92bb6-123">Zero tolerância bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="92bb6-123">Zero tolerance blocks all unknown executables</span></span>|





