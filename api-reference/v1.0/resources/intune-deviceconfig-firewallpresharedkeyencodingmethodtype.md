---
title: tipo de enumeração firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 07ea8e7a3a5622446ab2c0126d21187f6d7ce3b9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359233"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="141d7-103">tipo de enumeração firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="141d7-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="141d7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="141d7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="141d7-105">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="141d7-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="141d7-106">Membros</span><span class="sxs-lookup"><span data-stu-id="141d7-106">Members</span></span>
|<span data-ttu-id="141d7-107">Membro</span><span class="sxs-lookup"><span data-stu-id="141d7-107">Member</span></span>|<span data-ttu-id="141d7-108">Valor</span><span class="sxs-lookup"><span data-stu-id="141d7-108">Value</span></span>|<span data-ttu-id="141d7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="141d7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="141d7-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="141d7-110">deviceDefault</span></span>|<span data-ttu-id="141d7-111">,0</span><span class="sxs-lookup"><span data-stu-id="141d7-111">0</span></span>|<span data-ttu-id="141d7-112">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="141d7-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="141d7-113">none</span><span class="sxs-lookup"><span data-stu-id="141d7-113">none</span></span>|<span data-ttu-id="141d7-114">1</span><span class="sxs-lookup"><span data-stu-id="141d7-114">1</span></span>|<span data-ttu-id="141d7-115">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="141d7-115">Preshared key is not encoded.</span></span> <span data-ttu-id="141d7-116">Em vez disso, ele é mantido em seu formato de caracteres largos</span><span class="sxs-lookup"><span data-stu-id="141d7-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="141d7-117">utF8</span><span class="sxs-lookup"><span data-stu-id="141d7-117">utF8</span></span>|<span data-ttu-id="141d7-118">duas</span><span class="sxs-lookup"><span data-stu-id="141d7-118">2</span></span>|<span data-ttu-id="141d7-119">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="141d7-119">Encode the preshared key using UTF-8</span></span>|




