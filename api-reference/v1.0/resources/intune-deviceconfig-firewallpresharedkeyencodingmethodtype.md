---
title: tipo de número firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 200177be7f8258965067f12cace3b163aefc6b78
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755053"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="f76a2-103">tipo de número firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="f76a2-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="f76a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f76a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f76a2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f76a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f76a2-106">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="f76a2-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="f76a2-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f76a2-107">Members</span></span>
|<span data-ttu-id="f76a2-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f76a2-108">Member</span></span>|<span data-ttu-id="f76a2-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f76a2-109">Value</span></span>|<span data-ttu-id="f76a2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f76a2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f76a2-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f76a2-111">deviceDefault</span></span>|<span data-ttu-id="f76a2-112">0</span><span class="sxs-lookup"><span data-stu-id="f76a2-112">0</span></span>|<span data-ttu-id="f76a2-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="f76a2-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="f76a2-114">nenhuma</span><span class="sxs-lookup"><span data-stu-id="f76a2-114">none</span></span>|<span data-ttu-id="f76a2-115">1</span><span class="sxs-lookup"><span data-stu-id="f76a2-115">1</span></span>|<span data-ttu-id="f76a2-116">A chave pré-compartilhada não está codificada.</span><span class="sxs-lookup"><span data-stu-id="f76a2-116">Preshared key is not encoded.</span></span> <span data-ttu-id="f76a2-117">Em vez disso, ele é mantido em seu formato de caractere largo</span><span class="sxs-lookup"><span data-stu-id="f76a2-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="f76a2-118">utF8</span><span class="sxs-lookup"><span data-stu-id="f76a2-118">utF8</span></span>|<span data-ttu-id="f76a2-119">2</span><span class="sxs-lookup"><span data-stu-id="f76a2-119">2</span></span>|<span data-ttu-id="f76a2-120">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="f76a2-120">Encode the preshared key using UTF-8</span></span>|




