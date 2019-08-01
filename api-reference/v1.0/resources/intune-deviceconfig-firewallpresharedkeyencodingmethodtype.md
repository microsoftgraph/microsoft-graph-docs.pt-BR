---
title: tipo de enumeração firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a563d030a12480c6151a76cf2d58f743783bb378
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031539"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="9748f-103">tipo de enumeração firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="9748f-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="9748f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9748f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9748f-105">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="9748f-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="9748f-106">Membros</span><span class="sxs-lookup"><span data-stu-id="9748f-106">Members</span></span>
|<span data-ttu-id="9748f-107">Membro</span><span class="sxs-lookup"><span data-stu-id="9748f-107">Member</span></span>|<span data-ttu-id="9748f-108">Valor</span><span class="sxs-lookup"><span data-stu-id="9748f-108">Value</span></span>|<span data-ttu-id="9748f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9748f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9748f-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9748f-110">deviceDefault</span></span>|<span data-ttu-id="9748f-111">,0</span><span class="sxs-lookup"><span data-stu-id="9748f-111">0</span></span>|<span data-ttu-id="9748f-112">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="9748f-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="9748f-113">none</span><span class="sxs-lookup"><span data-stu-id="9748f-113">none</span></span>|<span data-ttu-id="9748f-114">1</span><span class="sxs-lookup"><span data-stu-id="9748f-114">1</span></span>|<span data-ttu-id="9748f-115">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="9748f-115">Preshared key is not encoded.</span></span> <span data-ttu-id="9748f-116">Em vez disso, ele é mantido em seu formato de caracteres largos</span><span class="sxs-lookup"><span data-stu-id="9748f-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="9748f-117">utF8</span><span class="sxs-lookup"><span data-stu-id="9748f-117">utF8</span></span>|<span data-ttu-id="9748f-118">duas</span><span class="sxs-lookup"><span data-stu-id="9748f-118">2</span></span>|<span data-ttu-id="9748f-119">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="9748f-119">Encode the preshared key using UTF-8</span></span>|



