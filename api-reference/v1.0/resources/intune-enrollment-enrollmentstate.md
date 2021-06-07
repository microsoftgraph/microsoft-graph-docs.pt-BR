---
title: Tipo de número de enrollmentState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 53b0ccc5f4605d888a056c8093e7d286441bc244
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756395"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="59889-103">Tipo de número de enrollmentState</span><span class="sxs-lookup"><span data-stu-id="59889-103">enrollmentState enum type</span></span>

<span data-ttu-id="59889-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59889-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59889-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59889-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59889-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="59889-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="59889-107">Membros</span><span class="sxs-lookup"><span data-stu-id="59889-107">Members</span></span>
|<span data-ttu-id="59889-108">Membro</span><span class="sxs-lookup"><span data-stu-id="59889-108">Member</span></span>|<span data-ttu-id="59889-109">Valor</span><span class="sxs-lookup"><span data-stu-id="59889-109">Value</span></span>|<span data-ttu-id="59889-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="59889-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59889-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="59889-111">unknown</span></span>|<span data-ttu-id="59889-112">0</span><span class="sxs-lookup"><span data-stu-id="59889-112">0</span></span>|<span data-ttu-id="59889-113">O estado de registro do dispositivo é desconhecido</span><span class="sxs-lookup"><span data-stu-id="59889-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="59889-114">inscrito</span><span class="sxs-lookup"><span data-stu-id="59889-114">enrolled</span></span>|<span data-ttu-id="59889-115">1</span><span class="sxs-lookup"><span data-stu-id="59889-115">1</span></span>|<span data-ttu-id="59889-116">O dispositivo está inscrito.</span><span class="sxs-lookup"><span data-stu-id="59889-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="59889-117">pendingReset</span><span class="sxs-lookup"><span data-stu-id="59889-117">pendingReset</span></span>|<span data-ttu-id="59889-118">2</span><span class="sxs-lookup"><span data-stu-id="59889-118">2</span></span>|<span data-ttu-id="59889-119">Inscrito, mas ele é inscrito por meio do perfil de registro e o perfil inscrito é diferente do perfil atribuído.</span><span class="sxs-lookup"><span data-stu-id="59889-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="59889-120">failed</span><span class="sxs-lookup"><span data-stu-id="59889-120">failed</span></span>|<span data-ttu-id="59889-121">3</span><span class="sxs-lookup"><span data-stu-id="59889-121">3</span></span>|<span data-ttu-id="59889-122">Não registrado e há registro de falha no registro.</span><span class="sxs-lookup"><span data-stu-id="59889-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="59889-123">notContacted</span><span class="sxs-lookup"><span data-stu-id="59889-123">notContacted</span></span>|<span data-ttu-id="59889-124">4 </span><span class="sxs-lookup"><span data-stu-id="59889-124">4</span></span>|<span data-ttu-id="59889-125">O dispositivo é importado, mas não está inscrito.</span><span class="sxs-lookup"><span data-stu-id="59889-125">Device is imported but not enrolled.</span></span>|




