---
title: tipo de enum defenderCloudBlockLevelType
description: Valores possíveis de nível de bloco de nuvem
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 13f8828478eb063eaa25d8561d5a254c86f4b856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924717"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="5299f-103">tipo de enum defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="5299f-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="5299f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5299f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5299f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5299f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5299f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5299f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5299f-107">Valores possíveis de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="5299f-107">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="5299f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5299f-108">Members</span></span>
|<span data-ttu-id="5299f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5299f-109">Member</span></span>|<span data-ttu-id="5299f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5299f-110">Value</span></span>|<span data-ttu-id="5299f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5299f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5299f-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="5299f-112">notConfigured</span></span>|<span data-ttu-id="5299f-113">0</span><span class="sxs-lookup"><span data-stu-id="5299f-113">0</span></span>|<span data-ttu-id="5299f-114">Valor padrão, usa o padrão de bloqueio de antivírus do Windows Defender nível e fornece detecção forte sem aumentar o risco de detecção legítimos arquivos</span><span class="sxs-lookup"><span data-stu-id="5299f-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="5299f-115">high</span><span class="sxs-lookup"><span data-stu-id="5299f-115">high</span></span>|<span data-ttu-id="5299f-116">1</span><span class="sxs-lookup"><span data-stu-id="5299f-116">1</span></span>|<span data-ttu-id="5299f-117">Alta aplica um alto nível de detecção.</span><span class="sxs-lookup"><span data-stu-id="5299f-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="5299f-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="5299f-118">highPlus</span></span>|<span data-ttu-id="5299f-119">2</span><span class="sxs-lookup"><span data-stu-id="5299f-119">2</span></span>|<span data-ttu-id="5299f-120">Alta + usa o alto nível e aplica as medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="5299f-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="5299f-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="5299f-121">zeroTolerance</span></span>|<span data-ttu-id="5299f-122">3</span><span class="sxs-lookup"><span data-stu-id="5299f-122">3</span></span>|<span data-ttu-id="5299f-123">Zero tolerância bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="5299f-123">Zero tolerance blocks all unknown executables</span></span>|





