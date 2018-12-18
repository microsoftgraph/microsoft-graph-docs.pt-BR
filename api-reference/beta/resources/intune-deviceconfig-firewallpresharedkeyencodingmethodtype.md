---
title: tipo de enum firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: tfitzmac
ms.openlocfilehash: 3ed2456f54bd27a3efa04d959edba48f7c100692
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324929"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="c6c15-103">tipo de enum firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="c6c15-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="c6c15-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c6c15-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6c15-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c6c15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6c15-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c6c15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6c15-107">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="c6c15-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="c6c15-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c6c15-108">Members</span></span>
|<span data-ttu-id="c6c15-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c6c15-109">Member</span></span>|<span data-ttu-id="c6c15-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c6c15-110">Value</span></span>|<span data-ttu-id="c6c15-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6c15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6c15-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c6c15-112">deviceDefault</span></span>|<span data-ttu-id="c6c15-113">0</span><span class="sxs-lookup"><span data-stu-id="c6c15-113">0</span></span>|<span data-ttu-id="c6c15-114">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="c6c15-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="c6c15-115">none</span><span class="sxs-lookup"><span data-stu-id="c6c15-115">none</span></span>|<span data-ttu-id="c6c15-116">1</span><span class="sxs-lookup"><span data-stu-id="c6c15-116">1</span></span>|<span data-ttu-id="c6c15-117">Chave pré compartilhada não é codificado.</span><span class="sxs-lookup"><span data-stu-id="c6c15-117">Preshared key is not encoded.</span></span> <span data-ttu-id="c6c15-118">Em vez disso, ele é mantido em seu formato de caractere largo</span><span class="sxs-lookup"><span data-stu-id="c6c15-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="c6c15-119">utF8</span><span class="sxs-lookup"><span data-stu-id="c6c15-119">utF8</span></span>|<span data-ttu-id="c6c15-120">2</span><span class="sxs-lookup"><span data-stu-id="c6c15-120">2</span></span>|<span data-ttu-id="c6c15-121">Codificar a chave pré compartilhada usando a codificação UTF-8</span><span class="sxs-lookup"><span data-stu-id="c6c15-121">Encode the preshared key using UTF-8</span></span>|





