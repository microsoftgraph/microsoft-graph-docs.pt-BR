---
title: tipo de enumeração firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0e2b5a3094ea0e5f351d67968254250156f98453
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526434"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="75359-103">tipo de enumeração firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="75359-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="75359-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="75359-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75359-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75359-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75359-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75359-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75359-107">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="75359-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="75359-108">Membros</span><span class="sxs-lookup"><span data-stu-id="75359-108">Members</span></span>
|<span data-ttu-id="75359-109">Membro</span><span class="sxs-lookup"><span data-stu-id="75359-109">Member</span></span>|<span data-ttu-id="75359-110">Valor</span><span class="sxs-lookup"><span data-stu-id="75359-110">Value</span></span>|<span data-ttu-id="75359-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="75359-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75359-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="75359-112">deviceDefault</span></span>|<span data-ttu-id="75359-113">,0</span><span class="sxs-lookup"><span data-stu-id="75359-113">0</span></span>|<span data-ttu-id="75359-114">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="75359-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="75359-115">nenhuma</span><span class="sxs-lookup"><span data-stu-id="75359-115">none</span></span>|<span data-ttu-id="75359-116">1 </span><span class="sxs-lookup"><span data-stu-id="75359-116">1</span></span>|<span data-ttu-id="75359-117">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="75359-117">Preshared key is not encoded.</span></span> <span data-ttu-id="75359-118">Em vez disso, ele é mantido em seu formato de caracteres largos</span><span class="sxs-lookup"><span data-stu-id="75359-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="75359-119">utF8</span><span class="sxs-lookup"><span data-stu-id="75359-119">utF8</span></span>|<span data-ttu-id="75359-120">2 </span><span class="sxs-lookup"><span data-stu-id="75359-120">2</span></span>|<span data-ttu-id="75359-121">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="75359-121">Encode the preshared key using UTF-8</span></span>|



