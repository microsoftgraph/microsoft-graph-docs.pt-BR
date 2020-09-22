---
title: tipo de enumeração firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e6ad3214eb16e69c6a3da7aa51a69cc8b43eca90
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056678"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="7ee76-103">tipo de enumeração firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="7ee76-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="7ee76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ee76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ee76-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ee76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ee76-106">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="7ee76-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="7ee76-107">Membros</span><span class="sxs-lookup"><span data-stu-id="7ee76-107">Members</span></span>
|<span data-ttu-id="7ee76-108">Membro</span><span class="sxs-lookup"><span data-stu-id="7ee76-108">Member</span></span>|<span data-ttu-id="7ee76-109">Valor</span><span class="sxs-lookup"><span data-stu-id="7ee76-109">Value</span></span>|<span data-ttu-id="7ee76-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ee76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ee76-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="7ee76-111">deviceDefault</span></span>|<span data-ttu-id="7ee76-112">,0</span><span class="sxs-lookup"><span data-stu-id="7ee76-112">0</span></span>|<span data-ttu-id="7ee76-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="7ee76-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="7ee76-114">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7ee76-114">none</span></span>|<span data-ttu-id="7ee76-115">1 </span><span class="sxs-lookup"><span data-stu-id="7ee76-115">1</span></span>|<span data-ttu-id="7ee76-116">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="7ee76-116">Preshared key is not encoded.</span></span> <span data-ttu-id="7ee76-117">Em vez disso, ele é mantido em seu formato de caracteres largos</span><span class="sxs-lookup"><span data-stu-id="7ee76-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="7ee76-118">utF8</span><span class="sxs-lookup"><span data-stu-id="7ee76-118">utF8</span></span>|<span data-ttu-id="7ee76-119">2 </span><span class="sxs-lookup"><span data-stu-id="7ee76-119">2</span></span>|<span data-ttu-id="7ee76-120">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="7ee76-120">Encode the preshared key using UTF-8</span></span>|









