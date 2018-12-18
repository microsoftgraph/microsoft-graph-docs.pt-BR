---
title: tipo de enum firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: tfitzmac
ms.openlocfilehash: b8ab119c58aec6e62c0a32ccf310f43eab029573
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343586"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="d31ff-103">tipo de enum firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="d31ff-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="d31ff-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d31ff-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d31ff-105">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="d31ff-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="d31ff-106">Membros</span><span class="sxs-lookup"><span data-stu-id="d31ff-106">Members</span></span>
|<span data-ttu-id="d31ff-107">Membro</span><span class="sxs-lookup"><span data-stu-id="d31ff-107">Member</span></span>|<span data-ttu-id="d31ff-108">Valor</span><span class="sxs-lookup"><span data-stu-id="d31ff-108">Value</span></span>|<span data-ttu-id="d31ff-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d31ff-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d31ff-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d31ff-110">deviceDefault</span></span>|<span data-ttu-id="d31ff-111">0</span><span class="sxs-lookup"><span data-stu-id="d31ff-111">0</span></span>|<span data-ttu-id="d31ff-112">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="d31ff-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d31ff-113">none</span><span class="sxs-lookup"><span data-stu-id="d31ff-113">none</span></span>|<span data-ttu-id="d31ff-114">1</span><span class="sxs-lookup"><span data-stu-id="d31ff-114">1</span></span>|<span data-ttu-id="d31ff-115">Chave pré compartilhada não é codificado.</span><span class="sxs-lookup"><span data-stu-id="d31ff-115">Preshared key is not encoded.</span></span> <span data-ttu-id="d31ff-116">Em vez disso, ele é mantido em seu formato de caractere largo</span><span class="sxs-lookup"><span data-stu-id="d31ff-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="d31ff-117">utF8</span><span class="sxs-lookup"><span data-stu-id="d31ff-117">utF8</span></span>|<span data-ttu-id="d31ff-118">2</span><span class="sxs-lookup"><span data-stu-id="d31ff-118">2</span></span>|<span data-ttu-id="d31ff-119">Codificar a chave pré compartilhada usando a codificação UTF-8</span><span class="sxs-lookup"><span data-stu-id="d31ff-119">Encode the preshared key using UTF-8</span></span>|



