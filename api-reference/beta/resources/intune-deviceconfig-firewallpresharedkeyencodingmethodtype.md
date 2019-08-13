---
title: tipo de enumeração firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 135509ba9ce5c85e8d4da308b66206f3cab4fe4e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338130"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="aea0a-103">tipo de enumeração firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="aea0a-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="aea0a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aea0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aea0a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aea0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aea0a-106">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="aea0a-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="aea0a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="aea0a-107">Members</span></span>
|<span data-ttu-id="aea0a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="aea0a-108">Member</span></span>|<span data-ttu-id="aea0a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="aea0a-109">Value</span></span>|<span data-ttu-id="aea0a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="aea0a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aea0a-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="aea0a-111">deviceDefault</span></span>|<span data-ttu-id="aea0a-112">,0</span><span class="sxs-lookup"><span data-stu-id="aea0a-112">0</span></span>|<span data-ttu-id="aea0a-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="aea0a-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="aea0a-114">none</span><span class="sxs-lookup"><span data-stu-id="aea0a-114">none</span></span>|<span data-ttu-id="aea0a-115">1</span><span class="sxs-lookup"><span data-stu-id="aea0a-115">1</span></span>|<span data-ttu-id="aea0a-116">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="aea0a-116">Preshared key is not encoded.</span></span> <span data-ttu-id="aea0a-117">Em vez disso, ele é mantido em seu formato de caracteres largos</span><span class="sxs-lookup"><span data-stu-id="aea0a-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="aea0a-118">utF8</span><span class="sxs-lookup"><span data-stu-id="aea0a-118">utF8</span></span>|<span data-ttu-id="aea0a-119">duas</span><span class="sxs-lookup"><span data-stu-id="aea0a-119">2</span></span>|<span data-ttu-id="aea0a-120">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="aea0a-120">Encode the preshared key using UTF-8</span></span>|



