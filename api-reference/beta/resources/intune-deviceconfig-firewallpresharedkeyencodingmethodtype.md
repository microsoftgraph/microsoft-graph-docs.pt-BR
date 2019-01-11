---
title: tipo de enum firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2dd5eb58c4fe2e8729ab1adc4aa55ad0c701157f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862150"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="706c3-103">tipo de enum firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="706c3-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="706c3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="706c3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="706c3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="706c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="706c3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="706c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="706c3-107">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="706c3-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="706c3-108">Membros</span><span class="sxs-lookup"><span data-stu-id="706c3-108">Members</span></span>
|<span data-ttu-id="706c3-109">Membro</span><span class="sxs-lookup"><span data-stu-id="706c3-109">Member</span></span>|<span data-ttu-id="706c3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="706c3-110">Value</span></span>|<span data-ttu-id="706c3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="706c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="706c3-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="706c3-112">deviceDefault</span></span>|<span data-ttu-id="706c3-113">0</span><span class="sxs-lookup"><span data-stu-id="706c3-113">0</span></span>|<span data-ttu-id="706c3-114">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="706c3-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="706c3-115">nenhum</span><span class="sxs-lookup"><span data-stu-id="706c3-115">none</span></span>|<span data-ttu-id="706c3-116">1</span><span class="sxs-lookup"><span data-stu-id="706c3-116">1</span></span>|<span data-ttu-id="706c3-117">Chave pré compartilhada não é codificado.</span><span class="sxs-lookup"><span data-stu-id="706c3-117">Preshared key is not encoded.</span></span> <span data-ttu-id="706c3-118">Em vez disso, ele é mantido em seu formato de caractere largo</span><span class="sxs-lookup"><span data-stu-id="706c3-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="706c3-119">utF8</span><span class="sxs-lookup"><span data-stu-id="706c3-119">utF8</span></span>|<span data-ttu-id="706c3-120">2</span><span class="sxs-lookup"><span data-stu-id="706c3-120">2</span></span>|<span data-ttu-id="706c3-121">Codificar a chave pré compartilhada usando a codificação UTF-8</span><span class="sxs-lookup"><span data-stu-id="706c3-121">Encode the preshared key using UTF-8</span></span>|





