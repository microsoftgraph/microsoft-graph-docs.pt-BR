---
title: tipo de enumeração firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dadb35cb95db83c03c74bdb2e4eac70a5951cc5e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532515"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="ed382-103">tipo de enumeração firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="ed382-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="ed382-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed382-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed382-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed382-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed382-106">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="ed382-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="ed382-107">Membros</span><span class="sxs-lookup"><span data-stu-id="ed382-107">Members</span></span>
|<span data-ttu-id="ed382-108">Membro</span><span class="sxs-lookup"><span data-stu-id="ed382-108">Member</span></span>|<span data-ttu-id="ed382-109">Valor</span><span class="sxs-lookup"><span data-stu-id="ed382-109">Value</span></span>|<span data-ttu-id="ed382-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed382-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed382-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ed382-111">deviceDefault</span></span>|<span data-ttu-id="ed382-112">,0</span><span class="sxs-lookup"><span data-stu-id="ed382-112">0</span></span>|<span data-ttu-id="ed382-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="ed382-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="ed382-114">nenhuma</span><span class="sxs-lookup"><span data-stu-id="ed382-114">none</span></span>|<span data-ttu-id="ed382-115">1 </span><span class="sxs-lookup"><span data-stu-id="ed382-115">1</span></span>|<span data-ttu-id="ed382-116">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="ed382-116">Preshared key is not encoded.</span></span> <span data-ttu-id="ed382-117">Em vez disso, ele é mantido em seu formato de caracteres largos</span><span class="sxs-lookup"><span data-stu-id="ed382-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="ed382-118">utF8</span><span class="sxs-lookup"><span data-stu-id="ed382-118">utF8</span></span>|<span data-ttu-id="ed382-119">2 </span><span class="sxs-lookup"><span data-stu-id="ed382-119">2</span></span>|<span data-ttu-id="ed382-120">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="ed382-120">Encode the preshared key using UTF-8</span></span>|




