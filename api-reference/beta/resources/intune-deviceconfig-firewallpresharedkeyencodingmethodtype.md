---
title: tipo de enumeração firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36c49a0c97ac8f2e9267f20762fd6e748d952240
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556183"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="29fb3-103">tipo de enumeração firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="29fb3-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="29fb3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29fb3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29fb3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29fb3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29fb3-106">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="29fb3-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="29fb3-107">Membros</span><span class="sxs-lookup"><span data-stu-id="29fb3-107">Members</span></span>
|<span data-ttu-id="29fb3-108">Membro</span><span class="sxs-lookup"><span data-stu-id="29fb3-108">Member</span></span>|<span data-ttu-id="29fb3-109">Valor</span><span class="sxs-lookup"><span data-stu-id="29fb3-109">Value</span></span>|<span data-ttu-id="29fb3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="29fb3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29fb3-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="29fb3-111">deviceDefault</span></span>|<span data-ttu-id="29fb3-112">,0</span><span class="sxs-lookup"><span data-stu-id="29fb3-112">0</span></span>|<span data-ttu-id="29fb3-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="29fb3-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="29fb3-114">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="29fb3-114">none</span></span>|<span data-ttu-id="29fb3-115">1 </span><span class="sxs-lookup"><span data-stu-id="29fb3-115">1</span></span>|<span data-ttu-id="29fb3-116">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="29fb3-116">Preshared key is not encoded.</span></span> <span data-ttu-id="29fb3-117">Em vez disso, ele é mantido em seu formato de caracteres largos</span><span class="sxs-lookup"><span data-stu-id="29fb3-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="29fb3-118">utF8</span><span class="sxs-lookup"><span data-stu-id="29fb3-118">utF8</span></span>|<span data-ttu-id="29fb3-119">2 </span><span class="sxs-lookup"><span data-stu-id="29fb3-119">2</span></span>|<span data-ttu-id="29fb3-120">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="29fb3-120">Encode the preshared key using UTF-8</span></span>|





