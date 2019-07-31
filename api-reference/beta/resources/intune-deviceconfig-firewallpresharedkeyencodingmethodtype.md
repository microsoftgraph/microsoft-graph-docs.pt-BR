---
title: tipo de enumeração firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ddd167d69674c0e32c184aa0f68bd7698331ee3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004292"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="3e59e-103">tipo de enumeração firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="3e59e-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="3e59e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3e59e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e59e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e59e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e59e-106">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="3e59e-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="3e59e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3e59e-107">Members</span></span>
|<span data-ttu-id="3e59e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3e59e-108">Member</span></span>|<span data-ttu-id="3e59e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3e59e-109">Value</span></span>|<span data-ttu-id="3e59e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e59e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e59e-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3e59e-111">deviceDefault</span></span>|<span data-ttu-id="3e59e-112">,0</span><span class="sxs-lookup"><span data-stu-id="3e59e-112">0</span></span>|<span data-ttu-id="3e59e-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="3e59e-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="3e59e-114">none</span><span class="sxs-lookup"><span data-stu-id="3e59e-114">none</span></span>|<span data-ttu-id="3e59e-115">1</span><span class="sxs-lookup"><span data-stu-id="3e59e-115">1</span></span>|<span data-ttu-id="3e59e-116">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="3e59e-116">Preshared key is not encoded.</span></span> <span data-ttu-id="3e59e-117">Em vez disso, ele é mantido em seu formato de caracteres largos</span><span class="sxs-lookup"><span data-stu-id="3e59e-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="3e59e-118">utF8</span><span class="sxs-lookup"><span data-stu-id="3e59e-118">utF8</span></span>|<span data-ttu-id="3e59e-119">duas</span><span class="sxs-lookup"><span data-stu-id="3e59e-119">2</span></span>|<span data-ttu-id="3e59e-120">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="3e59e-120">Encode the preshared key using UTF-8</span></span>|





