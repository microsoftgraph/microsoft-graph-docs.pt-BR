---
title: tipo de enumeração firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 24407bb787e471340de8111fb6662b5f67ff610a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730634"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="ca550-103">tipo de enumeração firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="ca550-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="ca550-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca550-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca550-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca550-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca550-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca550-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca550-107">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="ca550-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="ca550-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ca550-108">Members</span></span>
|<span data-ttu-id="ca550-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ca550-109">Member</span></span>|<span data-ttu-id="ca550-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ca550-110">Value</span></span>|<span data-ttu-id="ca550-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca550-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca550-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ca550-112">deviceDefault</span></span>|<span data-ttu-id="ca550-113">,0</span><span class="sxs-lookup"><span data-stu-id="ca550-113">0</span></span>|<span data-ttu-id="ca550-114">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="ca550-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="ca550-115">none</span><span class="sxs-lookup"><span data-stu-id="ca550-115">none</span></span>|<span data-ttu-id="ca550-116">1</span><span class="sxs-lookup"><span data-stu-id="ca550-116">1</span></span>|<span data-ttu-id="ca550-117">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="ca550-117">Preshared key is not encoded.</span></span> <span data-ttu-id="ca550-118">Em vez disso, ele é mantido em seu formato de caracteres largos</span><span class="sxs-lookup"><span data-stu-id="ca550-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="ca550-119">utF8</span><span class="sxs-lookup"><span data-stu-id="ca550-119">utF8</span></span>|<span data-ttu-id="ca550-120">duas</span><span class="sxs-lookup"><span data-stu-id="ca550-120">2</span></span>|<span data-ttu-id="ca550-121">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="ca550-121">Encode the preshared key using UTF-8</span></span>|





