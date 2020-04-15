---
title: tipo de enumeração firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 61820ed71b6923ff464f25183f7408eea885b7af
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445947"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="28b90-103">tipo de enumeração firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="28b90-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="28b90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28b90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28b90-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28b90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28b90-106">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="28b90-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="28b90-107">Membros</span><span class="sxs-lookup"><span data-stu-id="28b90-107">Members</span></span>
|<span data-ttu-id="28b90-108">Membro</span><span class="sxs-lookup"><span data-stu-id="28b90-108">Member</span></span>|<span data-ttu-id="28b90-109">Valor</span><span class="sxs-lookup"><span data-stu-id="28b90-109">Value</span></span>|<span data-ttu-id="28b90-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="28b90-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28b90-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="28b90-111">deviceDefault</span></span>|<span data-ttu-id="28b90-112">,0</span><span class="sxs-lookup"><span data-stu-id="28b90-112">0</span></span>|<span data-ttu-id="28b90-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="28b90-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="28b90-114">nenhuma</span><span class="sxs-lookup"><span data-stu-id="28b90-114">none</span></span>|<span data-ttu-id="28b90-115">1</span><span class="sxs-lookup"><span data-stu-id="28b90-115">1</span></span>|<span data-ttu-id="28b90-116">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="28b90-116">Preshared key is not encoded.</span></span> <span data-ttu-id="28b90-117">Em vez disso, ele é mantido em seu formato de caracteres largos</span><span class="sxs-lookup"><span data-stu-id="28b90-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="28b90-118">utF8</span><span class="sxs-lookup"><span data-stu-id="28b90-118">utF8</span></span>|<span data-ttu-id="28b90-119">duas</span><span class="sxs-lookup"><span data-stu-id="28b90-119">2</span></span>|<span data-ttu-id="28b90-120">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="28b90-120">Encode the preshared key using UTF-8</span></span>|







