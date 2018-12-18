---
title: tipo de enum defenderCloudBlockLevelType
description: Valores possíveis de nível de bloco de nuvem
author: tfitzmac
ms.openlocfilehash: 19c101cc82673009a39d6545f7340fabf65b287a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326611"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="47a08-103">tipo de enum defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="47a08-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="47a08-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="47a08-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47a08-105">Valores possíveis de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="47a08-105">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="47a08-106">Membros</span><span class="sxs-lookup"><span data-stu-id="47a08-106">Members</span></span>
|<span data-ttu-id="47a08-107">Membro</span><span class="sxs-lookup"><span data-stu-id="47a08-107">Member</span></span>|<span data-ttu-id="47a08-108">Valor</span><span class="sxs-lookup"><span data-stu-id="47a08-108">Value</span></span>|<span data-ttu-id="47a08-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="47a08-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47a08-110">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="47a08-110">notConfigured</span></span>|<span data-ttu-id="47a08-111">0</span><span class="sxs-lookup"><span data-stu-id="47a08-111">0</span></span>|<span data-ttu-id="47a08-112">Valor padrão, usa o padrão de bloqueio de antivírus do Windows Defender nível e fornece detecção forte sem aumentar o risco de detecção legítimos arquivos</span><span class="sxs-lookup"><span data-stu-id="47a08-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="47a08-113">high</span><span class="sxs-lookup"><span data-stu-id="47a08-113">high</span></span>|<span data-ttu-id="47a08-114">1</span><span class="sxs-lookup"><span data-stu-id="47a08-114">1</span></span>|<span data-ttu-id="47a08-115">Alta aplica um alto nível de detecção.</span><span class="sxs-lookup"><span data-stu-id="47a08-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="47a08-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="47a08-116">highPlus</span></span>|<span data-ttu-id="47a08-117">2</span><span class="sxs-lookup"><span data-stu-id="47a08-117">2</span></span>|<span data-ttu-id="47a08-118">Alta + usa o alto nível e aplica as medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="47a08-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="47a08-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="47a08-119">zeroTolerance</span></span>|<span data-ttu-id="47a08-120">3</span><span class="sxs-lookup"><span data-stu-id="47a08-120">3</span></span>|<span data-ttu-id="47a08-121">Zero tolerância bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="47a08-121">Zero tolerance blocks all unknown executables</span></span>|



