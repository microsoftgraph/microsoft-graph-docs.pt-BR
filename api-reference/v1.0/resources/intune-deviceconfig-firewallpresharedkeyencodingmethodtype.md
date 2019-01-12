---
title: tipo de enum firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4ad59a11aec2fbf715657de95eb3aafc778da43a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947824"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="8e300-103">tipo de enum firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="8e300-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="8e300-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8e300-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e300-105">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="8e300-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="8e300-106">Membros</span><span class="sxs-lookup"><span data-stu-id="8e300-106">Members</span></span>
|<span data-ttu-id="8e300-107">Membro</span><span class="sxs-lookup"><span data-stu-id="8e300-107">Member</span></span>|<span data-ttu-id="8e300-108">Valor</span><span class="sxs-lookup"><span data-stu-id="8e300-108">Value</span></span>|<span data-ttu-id="8e300-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e300-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e300-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="8e300-110">deviceDefault</span></span>|<span data-ttu-id="8e300-111">0</span><span class="sxs-lookup"><span data-stu-id="8e300-111">0</span></span>|<span data-ttu-id="8e300-112">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="8e300-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="8e300-113">nenhum</span><span class="sxs-lookup"><span data-stu-id="8e300-113">none</span></span>|<span data-ttu-id="8e300-114">1</span><span class="sxs-lookup"><span data-stu-id="8e300-114">1</span></span>|<span data-ttu-id="8e300-115">Chave pré compartilhada não é codificado.</span><span class="sxs-lookup"><span data-stu-id="8e300-115">Preshared key is not encoded.</span></span> <span data-ttu-id="8e300-116">Em vez disso, ele é mantido em seu formato de caractere largo</span><span class="sxs-lookup"><span data-stu-id="8e300-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="8e300-117">utF8</span><span class="sxs-lookup"><span data-stu-id="8e300-117">utF8</span></span>|<span data-ttu-id="8e300-118">2</span><span class="sxs-lookup"><span data-stu-id="8e300-118">2</span></span>|<span data-ttu-id="8e300-119">Codificar a chave pré compartilhada usando a codificação UTF-8</span><span class="sxs-lookup"><span data-stu-id="8e300-119">Encode the preshared key using UTF-8</span></span>|



