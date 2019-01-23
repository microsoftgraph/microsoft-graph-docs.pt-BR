---
title: tipo de enum defenderCloudBlockLevelType
description: Valores possíveis de nível de bloco de nuvem
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b309184623cff19e44ee5afea311d46fa89210fb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425908"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="1bbf4-103">tipo de enum defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="1bbf4-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="1bbf4-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="1bbf4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1bbf4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1bbf4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1bbf4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="1bbf4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bbf4-107">Valores possíveis de nível de bloco de nuvem</span><span class="sxs-lookup"><span data-stu-id="1bbf4-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="1bbf4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1bbf4-108">Members</span></span>
|<span data-ttu-id="1bbf4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1bbf4-109">Member</span></span>|<span data-ttu-id="1bbf4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1bbf4-110">Value</span></span>|<span data-ttu-id="1bbf4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bbf4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bbf4-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="1bbf4-112">notConfigured</span></span>|<span data-ttu-id="1bbf4-113">0</span><span class="sxs-lookup"><span data-stu-id="1bbf4-113">0</span></span>|<span data-ttu-id="1bbf4-114">Valor padrão, usa o padrão de bloqueio de antivírus do Windows Defender nível e fornece detecção forte sem aumentar o risco de detecção legítimos arquivos</span><span class="sxs-lookup"><span data-stu-id="1bbf4-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="1bbf4-115">high</span><span class="sxs-lookup"><span data-stu-id="1bbf4-115">high</span></span>|<span data-ttu-id="1bbf4-116">1</span><span class="sxs-lookup"><span data-stu-id="1bbf4-116">1</span></span>|<span data-ttu-id="1bbf4-117">Alta aplica um alto nível de detecção.</span><span class="sxs-lookup"><span data-stu-id="1bbf4-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="1bbf4-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="1bbf4-118">highPlus</span></span>|<span data-ttu-id="1bbf4-119">2</span><span class="sxs-lookup"><span data-stu-id="1bbf4-119">2</span></span>|<span data-ttu-id="1bbf4-120">Alta + usa o alto nível e aplica as medidas de proteção de adição</span><span class="sxs-lookup"><span data-stu-id="1bbf4-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="1bbf4-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="1bbf4-121">zeroTolerance</span></span>|<span data-ttu-id="1bbf4-122">3</span><span class="sxs-lookup"><span data-stu-id="1bbf4-122">3</span></span>|<span data-ttu-id="1bbf4-123">Zero tolerância bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="1bbf4-123">Zero tolerance blocks all unknown executables</span></span>|




