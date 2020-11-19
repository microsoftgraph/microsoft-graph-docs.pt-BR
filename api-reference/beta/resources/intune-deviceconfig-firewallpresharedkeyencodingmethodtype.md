---
title: tipo de enumeração firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 79fcb89a8165cbea6d2132eda256c742231fd129
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303213"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="7b7c2-103">tipo de enumeração firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="7b7c2-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="7b7c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b7c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b7c2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7b7c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b7c2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b7c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b7c2-107">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="7b7c2-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="7b7c2-108">Membros</span><span class="sxs-lookup"><span data-stu-id="7b7c2-108">Members</span></span>
|<span data-ttu-id="7b7c2-109">Membro</span><span class="sxs-lookup"><span data-stu-id="7b7c2-109">Member</span></span>|<span data-ttu-id="7b7c2-110">Valor</span><span class="sxs-lookup"><span data-stu-id="7b7c2-110">Value</span></span>|<span data-ttu-id="7b7c2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b7c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b7c2-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="7b7c2-112">deviceDefault</span></span>|<span data-ttu-id="7b7c2-113">,0</span><span class="sxs-lookup"><span data-stu-id="7b7c2-113">0</span></span>|<span data-ttu-id="7b7c2-114">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="7b7c2-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="7b7c2-115">nenhum</span><span class="sxs-lookup"><span data-stu-id="7b7c2-115">none</span></span>|<span data-ttu-id="7b7c2-116">1</span><span class="sxs-lookup"><span data-stu-id="7b7c2-116">1</span></span>|<span data-ttu-id="7b7c2-117">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="7b7c2-117">Preshared key is not encoded.</span></span> <span data-ttu-id="7b7c2-118">Em vez disso, ele é mantido em seu formato de caracteres largos</span><span class="sxs-lookup"><span data-stu-id="7b7c2-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="7b7c2-119">utF8</span><span class="sxs-lookup"><span data-stu-id="7b7c2-119">utF8</span></span>|<span data-ttu-id="7b7c2-120">duas</span><span class="sxs-lookup"><span data-stu-id="7b7c2-120">2</span></span>|<span data-ttu-id="7b7c2-121">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="7b7c2-121">Encode the preshared key using UTF-8</span></span>|




