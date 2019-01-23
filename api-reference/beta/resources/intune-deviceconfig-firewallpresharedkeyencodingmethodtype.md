---
title: tipo de enum firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 577925f141c6dd94b493664d3617df939d19c5c6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410949"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="aa8d1-103">tipo de enum firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="aa8d1-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="aa8d1-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="aa8d1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aa8d1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aa8d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa8d1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="aa8d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa8d1-107">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="aa8d1-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="aa8d1-108">Membros</span><span class="sxs-lookup"><span data-stu-id="aa8d1-108">Members</span></span>
|<span data-ttu-id="aa8d1-109">Membro</span><span class="sxs-lookup"><span data-stu-id="aa8d1-109">Member</span></span>|<span data-ttu-id="aa8d1-110">Valor</span><span class="sxs-lookup"><span data-stu-id="aa8d1-110">Value</span></span>|<span data-ttu-id="aa8d1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa8d1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa8d1-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="aa8d1-112">deviceDefault</span></span>|<span data-ttu-id="aa8d1-113">0</span><span class="sxs-lookup"><span data-stu-id="aa8d1-113">0</span></span>|<span data-ttu-id="aa8d1-114">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="aa8d1-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="aa8d1-115">none</span><span class="sxs-lookup"><span data-stu-id="aa8d1-115">none</span></span>|<span data-ttu-id="aa8d1-116">1</span><span class="sxs-lookup"><span data-stu-id="aa8d1-116">1</span></span>|<span data-ttu-id="aa8d1-117">Chave pré compartilhada não é codificado.</span><span class="sxs-lookup"><span data-stu-id="aa8d1-117">Preshared key is not encoded.</span></span> <span data-ttu-id="aa8d1-118">Em vez disso, ele é mantido em seu formato de caractere largo</span><span class="sxs-lookup"><span data-stu-id="aa8d1-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="aa8d1-119">utF8</span><span class="sxs-lookup"><span data-stu-id="aa8d1-119">utF8</span></span>|<span data-ttu-id="aa8d1-120">2</span><span class="sxs-lookup"><span data-stu-id="aa8d1-120">2</span></span>|<span data-ttu-id="aa8d1-121">Codificar a chave pré compartilhada usando a codificação UTF-8</span><span class="sxs-lookup"><span data-stu-id="aa8d1-121">Encode the preshared key using UTF-8</span></span>|




