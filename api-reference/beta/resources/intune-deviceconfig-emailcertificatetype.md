---
title: tipo de enumeração emailCertificateType
description: Fontes de certificado com suporte para assinatura e criptografia de email.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7dbf484473643eff30463cb8c4dc8217113ab713
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791811"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="f0665-103">tipo de enumeração emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="f0665-103">emailCertificateType enum type</span></span>

> <span data-ttu-id="f0665-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0665-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0665-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0665-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0665-106">Fontes de certificado com suporte para assinatura e criptografia de email.</span><span class="sxs-lookup"><span data-stu-id="f0665-106">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="f0665-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f0665-107">Members</span></span>
|<span data-ttu-id="f0665-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f0665-108">Member</span></span>|<span data-ttu-id="f0665-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f0665-109">Value</span></span>|<span data-ttu-id="f0665-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0665-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0665-111">none</span><span class="sxs-lookup"><span data-stu-id="f0665-111">none</span></span>|<span data-ttu-id="f0665-112">,0</span><span class="sxs-lookup"><span data-stu-id="f0665-112">0</span></span>|<span data-ttu-id="f0665-113">Não use um certificado como fonte.</span><span class="sxs-lookup"><span data-stu-id="f0665-113">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="f0665-114">certificado</span><span class="sxs-lookup"><span data-stu-id="f0665-114">certificate</span></span>|<span data-ttu-id="f0665-115">1</span><span class="sxs-lookup"><span data-stu-id="f0665-115">1</span></span>|<span data-ttu-id="f0665-116">Usar um certificado para a fonte do certificado.</span><span class="sxs-lookup"><span data-stu-id="f0665-116">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="f0665-117">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="f0665-117">derivedCredential</span></span>|<span data-ttu-id="f0665-118">duas</span><span class="sxs-lookup"><span data-stu-id="f0665-118">2</span></span>|<span data-ttu-id="f0665-119">Use uma credencial derivada para a fonte do certificado.</span><span class="sxs-lookup"><span data-stu-id="f0665-119">Use a derived credential for certificate source.</span></span>|



