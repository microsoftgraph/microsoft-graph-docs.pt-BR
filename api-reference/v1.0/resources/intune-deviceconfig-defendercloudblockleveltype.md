---
title: tipo de enum defenderCloudBlockLevelType
description: Valores possíveis de nível de bloco de nuvem
ms.openlocfilehash: 6ea336418a90a3d4caeab074cb71fce997ea1275
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005442"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="b1ac1-103">tipo de enum defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="b1ac1-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="b1ac1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b1ac1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1ac1-105">Valores possíveis de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="b1ac1-105">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="b1ac1-106">Membros</span><span class="sxs-lookup"><span data-stu-id="b1ac1-106">Members</span></span>
|<span data-ttu-id="b1ac1-107">Membro</span><span class="sxs-lookup"><span data-stu-id="b1ac1-107">Member</span></span>|<span data-ttu-id="b1ac1-108">Valor</span><span class="sxs-lookup"><span data-stu-id="b1ac1-108">Value</span></span>|<span data-ttu-id="b1ac1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1ac1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1ac1-110">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="b1ac1-110">notConfigured</span></span>|<span data-ttu-id="b1ac1-111">0</span><span class="sxs-lookup"><span data-stu-id="b1ac1-111">0</span></span>|<span data-ttu-id="b1ac1-112">Valor padrão, usa o padrão de bloqueio de antivírus do Windows Defender nível e fornece detecção forte sem aumentar o risco de detecção legítimos arquivos</span><span class="sxs-lookup"><span data-stu-id="b1ac1-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="b1ac1-113">high</span><span class="sxs-lookup"><span data-stu-id="b1ac1-113">high</span></span>|<span data-ttu-id="b1ac1-114">1</span><span class="sxs-lookup"><span data-stu-id="b1ac1-114">1</span></span>|<span data-ttu-id="b1ac1-115">Alta aplica um alto nível de detecção.</span><span class="sxs-lookup"><span data-stu-id="b1ac1-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="b1ac1-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="b1ac1-116">highPlus</span></span>|<span data-ttu-id="b1ac1-117">2</span><span class="sxs-lookup"><span data-stu-id="b1ac1-117">2</span></span>|<span data-ttu-id="b1ac1-118">Alta + usa o alto nível e aplica as medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="b1ac1-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="b1ac1-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="b1ac1-119">zeroTolerance</span></span>|<span data-ttu-id="b1ac1-120">3</span><span class="sxs-lookup"><span data-stu-id="b1ac1-120">3</span></span>|<span data-ttu-id="b1ac1-121">Zero tolerância bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="b1ac1-121">Zero tolerance blocks all unknown executables</span></span>|



