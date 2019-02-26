---
title: tipo de enumeração firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c62144ef2974da5a3d975c759bb8d2bd2be6032
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259546"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="07528-103">tipo de enumeração firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="07528-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="07528-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07528-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07528-105">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="07528-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="07528-106">Membros</span><span class="sxs-lookup"><span data-stu-id="07528-106">Members</span></span>
|<span data-ttu-id="07528-107">Membro</span><span class="sxs-lookup"><span data-stu-id="07528-107">Member</span></span>|<span data-ttu-id="07528-108">Valor</span><span class="sxs-lookup"><span data-stu-id="07528-108">Value</span></span>|<span data-ttu-id="07528-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="07528-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07528-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="07528-110">deviceDefault</span></span>|<span data-ttu-id="07528-111">,0</span><span class="sxs-lookup"><span data-stu-id="07528-111">0</span></span>|<span data-ttu-id="07528-112">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="07528-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="07528-113">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="07528-113">none</span></span>|<span data-ttu-id="07528-114">1</span><span class="sxs-lookup"><span data-stu-id="07528-114">1</span></span>|<span data-ttu-id="07528-115">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="07528-115">Preshared key is not encoded.</span></span> <span data-ttu-id="07528-116">Em vez disso, ele é mantido em seu formato de caracteres largos</span><span class="sxs-lookup"><span data-stu-id="07528-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="07528-117">utF8</span><span class="sxs-lookup"><span data-stu-id="07528-117">utF8</span></span>|<span data-ttu-id="07528-118">duas</span><span class="sxs-lookup"><span data-stu-id="07528-118">2</span></span>|<span data-ttu-id="07528-119">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="07528-119">Encode the preshared key using UTF-8</span></span>|



